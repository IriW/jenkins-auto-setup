# jenkins-auto-setup
Create VM with Vagrant and configure Jenkins with Ansible

Prerequisites:

- Vagrant
- Ansible

## How does it work:

Initiate provisioning running `vagrant up`.

Once VM is provisioned, ansible role for Jenkins installation is triggered.

When Jenkins configuration is completed, the initial admin passwordpassword output will be displayed.
