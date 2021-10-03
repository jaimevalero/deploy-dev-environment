# Defaults installs for getting dev environment


## Installation
```bash
ansible-galaxy install -r requirements.yml

ansible-playbook install.yml --tags crons
```


### Debugging
```bash
ansible-playbook install.yml --skip-tags "packages"

ansible-playbook install.yml -tags crons
```

