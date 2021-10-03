# Defaults installs for getting dev environment

## App Installed:
* Skype, Teams.

* VSCode

* Docker 
  * Docker community Edition  
  * Compose
  * Containerd

* Package Managers
    Conda, YARN, NPM

* Languages    
    GO, Python, Node, Developer Tools (C, Make)

* VPN:
  * AnyConnect with autoconnect

* Other :   
  * Wifi Drivers
  * NVidia Drivers
  * Lots of alias
  * Hugo
  * Howdoi





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

