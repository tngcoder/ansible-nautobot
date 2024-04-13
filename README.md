# Ansible Nautobot installation
This is a repository for a small project to install Nautobot and all its dependency with Ansible. This project is not a module to manage Nautobot once it's installed

# using the playbooks
The project includes some playbook that are not specifically linked to the installation of Nautobot with ansible.
the "update.yml" and "letencrypt.yml" are generic playbook to prepare a host that will run nautobot.

the "nautobot.yml" playbook is a monolithic playbook that will install the prerequisites for Nautobot, Nautobot itself, and create a Nautobot configuration file.

The playbook could be simplified and split in many playbooks, (Example, a separate playbook to setup postgres database, another one to setup nginx, etc.), but this is my first attempt to deploy Nautobot automatically via Ansible. 

Any suggestions are more than welcome.
