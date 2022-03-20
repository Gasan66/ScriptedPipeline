# Elastic, kibana and filebeat's ansible playbook
This playbook will install elasticsearch, kibana and filebeat at targeted hosts 

A few of the things these playbooks accomplish:
- Install Elasticsearch
  - Upload from remote URL
  - Install rpm
- Install Kibana
  - Upload from remote URL
  - Install rpm
- Install filebeat
  - Upload from remote URL
  - Install rpm

Playbook has some parameters:
- all
  - elk_stack_version