# This repo is for my Development Environment, it contains all files necessary for auto-configuration

## Requirements
* Unbuntu 16.04 or latest
* Docker for $UBUNTU_VERSION (and its dependencies)
* Ansible (will run in docker) -> Python dependencies needed on localhost as well #todo
* Git (installed by default)

### Profile folder

This folder is used for basic profile configuration such as :

* ~/.profile 
* ~/.bash_profile
* ~/.bashrc
* Vim configuration and probably just the list of installed plugins

### Playbooks folder
#### Everything will be separated in roles / tasks with a global playbook according to ansible best practices

All the necessary playbooks used to keep the env up to date with tools and configs are kept here

* Up-to-date OS (Ubuntu 16.04 LTS)
    * apt-get update
    * Latest VIM
* Java (8 or later, via PPA)
* Netbeans (8.1 or later)
* Node + NPM (no NVM for now)
    * Yeoman
    * Yeoman generator for basic webapp
    * Gulp
    * Bower
* Ruby 
* Jekyll
* Php
* Wordpress
* Atom.io
    * Find a way to automate package installation ?
    * Find a way to automate configuration - if present

### Docker images folder
#### One sub-folder for every image

* Ansible
* youtube-dl
* Linters / Code Checkers
    * ESLint / JSHint
    * CSSLint
    * Checkstyle
    * Findbugs
* Tomcat (8 or later)
* Nginx (latest)
    * Configured for Python
    * Configured for PHP

