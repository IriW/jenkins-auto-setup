# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "base"
  config.vm.network "forwarded_port", guest: 8080, host: 8080
  config.vm.synced_folder "../vagrant_data", "/vagrant_data"
  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
  end
 
  config.vm.box = "ubuntu/focal64"
  config.vm.hostname = "jenkins-ubuntu20"
  config.vm.provision "shell" do |shell|
    shell.path = "jenkins.sh"
  end
end