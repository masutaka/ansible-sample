# a sample of Ansible

## Setup

Install VirtualBox and Vagrant.

Add ansible to your PC. For example,

    $ brew install ansible

Add the following to your ~/.ssh/config

```
Host melody
  HostName 127.0.0.1
  User vagrant
  Port 2222
  UserKnownHostsFile /dev/null
  StrictHostKeyChecking no
  PasswordAuthentication no
  IdentityFile "~/.vagrant.d/insecure_private_key"
  IdentitiesOnly yes
```

Boot vagrant

    $ vagrant up

Check to be able to execute `ssh` command.

    $ ssh melody

## Do Ansible

Checking

    $ ansible-playbook -C server.yml

Do ansible!

    $ ansible-playbook server.yml
