# Defaults installs for getting dev environment

## App Installed:
* Skype, Teams.

* VSCode

* Docker 
    Compose, Container

* Package Managers
    Conda, YARN

* Languages    
    GO, Python, NPM, Developer Tools (C, Make)

* Other :   
  * Wifi Drivers
  * NVidia Drivers
  * Lots of alias
  * Hugo
  * Howdoi

* VPN:
  * AnyConnect with autoconnect



## Installation
```bash
ansible-galaxy install -r requirements.yml

ansible-playbook install.yml 
```


### Debugging
```bash
ansible-playbook install.yml --skip-tags "packages"

ansible-playbook install.yml -tags crons
```

