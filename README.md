# Ansible EC2-Instance from Playbook
 
This playbook is for creating and configuring EC2 Instance on AWS Account using ansible-playbook. 

## Notes and requirements

 - The playbook was built and tested on Ubuntu 16.04 VMs, for EC2 Instance. 
 - You will need Ansible installed and running
 - Playbook is currently configured to set up the EC2 instance from ubuntu16.04.we gave in the playbook screetkey and password and region and etc,information.
 
 ## Instructions
 
 1. Edit your Ansible hosts file ('/etc/ansible/hosts') and add an 'elkservers' entry for the server you wish to install ELK on. You can of course name the host any way you want, this is just an example. 
 2. Verify connectivity to the EC2 server.
 3. In the terminal on the machine hosting Ansible, clone this repo.
 4. Cd into the directory, and run:
 `ansible-playbook ec2sample.yml`
 
 The plays in the playbook will run on the target server, installing ELK and the specified beats shippers. 
 
[site.yml]: https://github.com/DanielBerman/ansible-elk-playbook/blob/master/site.yml
