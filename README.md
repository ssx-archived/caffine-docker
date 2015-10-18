# Caffine
Caffine is a simple LAMP environment, provisioning handled by ansible with docker 
and virtualbox providers for local development. The components are:
  
  - [Ansible playbooks](https://github.com/ssx/caffine-ansible)
  - [Dockerfile to build image](https://github.com/ssx/caffine-docker)
  - [Vagrantfile to build for Virtualbox](https://github.com/ssx/caffine-virtualbox)
        
---

# Development Stack
This stack contains PHP5.6, nginx, node, composer and more. For a full picture, 
take a look through the Ansible playbooks.

---

# Use without building
If you wish to use this development environment without building the images, use the 
Dockerhub hosted image:
 
    docker run -itP hellossx/lamp 
 
---

# Pull Ansible submodules
You'll need to pull in the shared ansible scripts, using:

    git submodules init
    git submodules update


This should create/update the `ansible` directory which contains the playbooks 
used to configure the development environment.