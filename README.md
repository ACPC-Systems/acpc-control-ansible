# ACPC Control server ansible playbook
A repo contains the ansible playbook tree. The playbook contains of tasks and roles. The main task is found under files/control.yml,
while the control role is found under role directory. The control playbook runs only on localhost.

# Requirements:
  * Internet connection
  * Fresh ubuntu box installation
  * Downloading capability

# Installation
  * sudo apt update
  * sudo apt -y install git-hub python-pip
  * sudo pip install ansible
  * mkdir ansible
  * cd ansible
  * github clone https://github.com/ACM-ACPC/acpc-control-ansible

# Usage
  * cd acpc-control-ansible
  * ansible-playbook files/control.yml



