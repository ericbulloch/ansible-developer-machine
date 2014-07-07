ansible-developer-machine
=========================

This is a set of Ansible files to set up my developer machine.

You can install ansible on Ubuntu by running the following:
sudo apt-get install ansible

Ansible works using ssh. Make sure your user has an ssh key on your development machine.

You can change your development machine's IP address in the hosts file.
For my development machine I switch the IP address to 127.0.0.1
The hosts file should be placed in /etc/ansible/hosts

To run a specific playbook run the following:
ansible-playbook playbook

Examples:
ansible-playbook bashrc.yml
ansible-playbook packages.yml
ansible-playbook django.yml
ansible-playbook hipchat.yml
ansible-playbook vim.yml
ansible-playbook sublime.yml
ansible-playbook pycharm.yml
