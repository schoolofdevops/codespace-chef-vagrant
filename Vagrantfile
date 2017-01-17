# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "codespace-chef"
  config.vm.hostname = "codespace-chef"

  config.vm.network "private_network", ip: "192.168.51.10"
 
 config.vm.provider "virtualbox" do |vb|

  #   vb.gui = true
    vb.cpus = "2"
    vb.memory = "2048"
  end

  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
