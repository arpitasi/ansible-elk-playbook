
# Ansible ELK Playbook

This playbook is for setting up Elastic Search along with logstash and kibana (ELK stack) on a remote server.

## Notes and requirements

 - The playbook was built and tested on AWS ec2 instance based on Ubuntu  AMI
 - You will need Ansible installed and running
 - Playbook is currently configured to set up the ELK stack together with Metricbeat for server performance monitoring.

 ## Instructions

Please run ansible-playbook -i /opt/ansible/inventory/aws_ec2.yaml main.yml -vvvv --ask-vault-pass
Password for vault : awssecret

 The plays in the playbook will run on the Ansible Controller on target host set in dynamic inventory server, installing ELK and the specified hosts.
