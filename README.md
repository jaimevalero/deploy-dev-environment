# Ansible role for prepare my dev environment


## App Installed:

* Messenger app
  * Skype 
  * Teams

* GUI 
  * VSCode

* Docker 
  * Docker community Edition  
  * Compose
  * Containerd

* Package Managers
  * Conda
  * YARN
  * NPM

* Cloud
  * Aws-cli
  * Terraform 

* Languages    
  * GO, 
  * Python
  * Node
  * Developer Tools (C, Make)

* VPN:
  * AnyConnect with autoconnect

* Other :   
  * Wifi Drivers
  * NVidia Drivers
  * Lots of alias
  * Hugo
  * Howdoi


* TODO:
  * Openshift, 
  * cuDNN Library for Linux 

## Installation
```bash

# First install python3 to have ansible collections (ansible v2.9 or above)

ansible-playbook pre-works.yml 


#ansible-galaxy install -r requirements.yml

/usr/local/bin/ansible-galaxy  install -r requirements.yml

/usr/local/bin/ansible-playbook install.yml 

```


### Debugging
```bash
ansible-playbook install.yml --skip-tags "packages"

ansible-playbook install.yml -tags crons
```

from inside a container
```bash

docker run -it  -v $PWD:/applinuxmintd/mint19.1-amd64 bash

```
and then
```bash


cd /app
ansible-playbook pre-works.yml
/usr/local/bin/ansible-galaxy  install -r requirements.yml
/usr/local/bin/ansible-playbook install.yml 



```
