# Defaults installs for getting dev environment


## Installation
ansible-playbook install.yml --tags crons


### Debugging

ansible-playbook install.yml --skip-tags "packages"

ansible-playbook install.yml -tags crons

