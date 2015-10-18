# caffine-virtualbox
Caffine is a simple LAMP environment, provisioning handled by ansible with docker 
and virtualbox providers for local development.


# Development Stack
This stack contains PHP5.6, nginx, node, composer and more. For a full picture, 
take a look through the Ansible playbooks.


# Pull Ansible submodules
You'll need to pull in the shared ansible scripts, using:

    git submodules init
    git submodules update


This should create/update the `ansible` directory which contains the playbooks 
used to configure the development environment.