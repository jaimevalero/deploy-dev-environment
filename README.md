
# Defaults installs for getting dev environment





## Installation
ansible-galaxy install -r requirements.yml
ansible-playbook install-defaults.yaml 
ansible-playbook install-roles.yaml  


### Debugging
ansible-playbook install-defaults.yaml  --skip-tags "packages"
