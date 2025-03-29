# jenkins-auto-setup
Create VM with Vagrant and configure Jenkins with Ansible

Prerequisites:

- Vagrant
- Ansible / optional depending on installation tool chosen (ansible role, or bash script).

 If not installed: `sudo apt update && sudo apt install -y ansible`

- Ansible `jenkins` role from `geerlingguy` installed: `ansible-galaxy install geerlingguy.jenkins`. Confirm `ansible-galaxy list`

## How does it work:

Initiate provisioning running `vagrant up`.

1. If Vagrantfile specifies provisioning with bash script (here, the default one), the script will run and install&configure Jenkins.

2. If Vagrantfile has defined provisioning `ansible`, once VM is provisioned, ansible role for Jenkins installation is triggered.

When Jenkins configuration is completed, the initial admin passwordpassword output will be displayed.
