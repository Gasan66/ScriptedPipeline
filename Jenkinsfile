node("docker"){
    stage("Git checkout"){
        git credentialsId: '1a426d9e-fab0-4b28-9fd6-f20ea93a78e2', url: 'git@github.com:Gasan66/for_jenkins_test.git'
    }
    stage("Sample define secret_check"){
        secret_check=true
    }
    stage("Run playbook"){
        if (secret_check){
            sh 'ansible-playbook site.yml -i inventory/prod.yml'
        }
        else{
            echo 'need more action'
        }
        
    }
}