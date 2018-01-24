## Setup
In order to use Ansible roles you first have to install Ansible. You can install Ansible using the install_ansible script or using sudo apt-get install ansible. To run the roles you just need to excute the playbook. You can test the ansible roles using a dry test or test it inside a VM. 

## Install using install_ansible.sh script

(gives script excute permissions)

1. Type chmod +x install_ansible.sh 
2. Type ./install_ansible.sh to run

## Install using install_ansible_container.sh script
(gives script excute permissions)

1. Type chmod +x install_ansible_container.sh
2. Type ./install_ansible_container.sh to run

## Install ansible without script

1. sudo apt-get install software-properties-common
2. sudo apt-add-repository ppa:ansible/ansible
3. sudo apt-get update
4. sudo apt-get install ansible

## Install ansible container without script

1. sudo apt-get install python-pip python-dev build-essential
2. sudo pip install --upgrade pip
3. sudo pip install ansible-container[docker]

## Executing

To run the playbook simply execute the following command:

* ansible-playbook -K -c local -i inventory playbook.yml

## Testing Dry test - This will just check the playbook for issues

* ansible-playbook -K -c local -i inventory playbook.yml --check

## Installing Vagrant for testing Ansible roles
First you need to install VirtualBox using the sudo apt-get install virtualbox command.
You can either run the playbook or go to [here](https://www.vagrantup.com/docs/installation/) to download and install vargrant. 

## Testing in vagrant new VM

1. chmod +x testAnsibleInVagrant.sh
2. ./testAnsibleInVagrant.sh

## Testing in vagrant existing VM

1. chmod +x testAnsibleInVagrantExistingVM.sh
2. ./testAnsibleInVagrantExistingVM.sh

## Testing in container

1. Use the **ansible-container build** command 


