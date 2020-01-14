# ACPC Control server ansible playbook
A repo contains the ansible playbook tree. The playbook contains of tasks and roles. The main task is found under files/control.yml,
while the control role is found under role directory. The control playbook runs only on localhost.

# Requirements:
  * Internet connection
  * Fresh ubuntu box installation
  * Downloading capability

# Installation
  * sudo apt update
  * sudo apt -y install git-hub python3-pip
  * sudo pip3 install ansible
  * mkdir ansible
  * cd ansible
  * git clone https://github.com/ACPC-Systems/acpc-control-ansible

# Usage
  * cd acpc-control-ansible
  * sudo ansible-playbook files/control.yml
  * sudo systemctl reboot

# Ubuntu mirror
To install the different roles of ACPC, the control needs a local copy of the ubuntu mirror which can be downloaded from the repo 
https://github.com/ACM-ACPC/acpc-control-mirror.
The mirror size is +90G depends on the distro and architecture(s). For X86-64 ubuntu mirror is around 85G. The control server looks for the mirror under directory /MirrorPool. Either download the mirror in this directory, or mount this directory to a different partition to be able to move this partition from VM to another. In case using a different partition, do not forget to add its mount point to /etc/fstab

