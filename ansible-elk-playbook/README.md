
# Ansible ELK Playbook

This playbook is for setting up Elastic Search along with logstash and kibana (ELK stack) on a remote server.

## Notes and requirements

 - The playbook was built and tested on AWS ec2 instance based on Ubuntu  AMI
 - You will need Ansible installed and running
 - Playbook is currently configured to set up the ELK stack together with Metricbeat for server perf monitoring.

 ## Instructions

 1. Edit your Ansible hosts file ('/etc/ansible/hosts') and add an 'hosts' entry for the server you wish to install ELK on
 2. Verify connectivity to the ELK server, ssh connectivity must be working.
 3. In the terminal on the machine hosting Ansible, clone this repo.
 4. Cd into the directory, and run:
 `ansible-playbook main.yml`

 The plays in the playbook will run on the target server, installing ELK and the specified hosts.
