# This repo is for my Development Environment, it contains all files necessary for auto-configuration

## Requirements
* Unbuntu 16.04 or latest
* Docker for $UBUNTU_VERSION (and its dependencies)
* Ansible (will run in docker) -> Python dependencies needed on localhost as well #todo
* Git (installed by default)

### Playbooks folder
#### Everything will be separated in roles / tasks with a global playbook according to ansible best practices

All the necessary playbooks used to keep the env up to date with tools and configs are kept here

* Up-to-date OS (Ubuntu 16.04 LTS)
    * apt-get update
    * Latest VIM
* Java (8 or later, via PPA)
* Netbeans (8.1 or later)
* Node + NPM (no NVM for now)

