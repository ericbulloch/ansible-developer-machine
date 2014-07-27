ansible-developer-machine
=========================

This is a set of Ansible files to set up my developer machine.

You can install ansible on Ubuntu by running the following:

`sudo apt-get install ansible`

You will need to have ssh running on your development machine and an ssh key for ansible to work correctly. Here are some commands to run to get things up and running:

```
sudo apt-get install openssh-server
ssh-keygen -t rsa
cd ~/.ssh/
cat id_rsa.pub >> authorized_keys
```

You can change your development machine's IP address in the hosts file.
For my development machine I switch the IP address to 127.0.0.1
The hosts file should be placed in /etc/ansible/hosts

To run a specific playbook run the following:

`ansible-playbook playbook`

Examples:

```
ansible-playbook bashrc.yml
ansible-playbook packages.yml
ansible-playbook django.yml
ansible-playbook hipchat.yml
ansible-playbook vim.yml
ansible-playbook sublime.yml
ansible-playbook pycharm.yml
```
