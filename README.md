Vagrant+Ansible: provision multiple separate playbooks
======================================================

- Vagrant creates one host in Virtualbox

- Vagrant launches Ansible to apply two separate playbooks consequently to the same host. Each playbook contains single role:
   
   - `apache-only.yml`: role ‘apache’
   - `php-only.yml`: role ‘php’
   - Each playbook is initiated as individual provisioning step in Vagrantfile and they are not aware of each other
   
