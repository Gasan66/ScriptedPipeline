node("docker"){
    stage("Git checkout"){
        git credentialsId: '1a426d9e-fab0-4b28-9fd6-f20ea93a78e2', url: 'git@github.com:Gasan66/ScriptedPipeline.git'
    }
    stage("If Prod"){
        prod_run = False
    }
    stage("Run playbook"){
        if (prod_run){
            sh 'ansible-playbook site.yml -i inventory/prod.yml'
        }
        else{
            echo 'ansible-playbook site.yml -i inventory/prod.yml --check --diff'
        }
        
    }
}