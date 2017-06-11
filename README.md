# This repo is for my Development Environment, it contains all files necessary for auto-configuration

# Requirements to run the playbook
* Unbuntu 16.04
* Ansible 2.3 [installation instructions](http://docs.ansible.com/ansible/intro_installation.html#latest-releases-via-apt-debian)

## Playbook content
### The playbook is configured to run on localhost in the provided **hosts** file

You need to run the playbook with the option to specify which hosts file to use (**-i**) and the option to ask for sudo password when needed (**--ask-sudo-pass**).
The following commands assume you are positioned in the "playbooks" directory.
```
ansible-playbook -i hosts --ask-sudo-pass devenv.yml
```
If you need to run the playbook in check mode only, add the (**--check**) option at the end
```
ansible-playbook -i hosts --ask-sudo-pass devenv.yml --check
```

The playbook installs and configures the following software :

* Up-to-date OS (Ubuntu 16.04 LTS)
    * Atom (with plugins)
        * language-docker
        * linter
        * platformio-ide-terminal
        * autocomplete-python
        * emmet
        * dash
    * Docker & docker-compose
    * dockerized redmine installation (from sameersbn)
    * dockerized wekan server (open-source trello)
    * dockerized eclipse (eclipse-che)
    * hugo
    * java (8)
    * maven (from latest archive, not apt)
    * node (from latest stable release)
    * pycharm
    * python (2 & 3)    
    * zeal (multiple docsets downloaded)
        * Ansible
        * Bootstrap (3 & 4)
        * Python (2 & 3)
        * D3JS
        * Flask
        * NodeJS
        * SVG
        * Jquery
        * Sass
        * WordPress
    * redshift (f.lux equivalent)
    * tlp (thinkpad power control utility)
    * vlc media player
    * clementine music player
    * latest git for ubuntu
    * latest geany for ubuntu
    * latest gparted for ubuntu
    * latest meld for ubuntu
    * latest vim for ubuntu

Also, it configures the **/opt** folder to be owned by the current user and to contain all docker, docker-compose projects and volume folders.
All downloaded docker-compose projects are automatically started.
