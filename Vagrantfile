# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
    config.vm.box = "mwrock/Windows2016"
    config.vm.network "private_network", ip: "10.10.1.10"
    config.vm.provider "virtualbox" do |vb|
      vb.cpus = 1
      vb.memory = "2048"
    end
    config.vm.provision "shell", path: "provisioning/winrm.ps1", privileged: true
  end
  