# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.provider "virtualbox"
  
    # Define VM 1
    config.vm.define "vm1" do |vm1|
      vm1.vm.box = "ubuntu/focal64"
      vm1.vm.hostname = "VM1"
      vm1.vm.network "private_network", ip: "192.168.56.101"
      vm1.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = 2
      end
      vm1.vm.provision "shell", inline: <<-SHELL
        sudo apt-get update
        sudo apt-get upgrade -y
        echo 'vagrant ALL=(ALL) NOPASSWD:ALL' | sudo tee /etc/sudoers.d/vagrant
      SHELL
    end
  
    # Define VM 2
    config.vm.define "vm2" do |vm2|
      vm2.vm.box = "ubuntu/focal64"
      vm2.vm.hostname = "VM2"
      vm2.vm.network "private_network", ip: "192.168.56.102"
      vm2.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = 2
      end
      vm2.vm.provision "shell", inline: <<-SHELL
        sudo apt-get update
        sudo apt-get upgrade -y
        echo 'vagrant ALL=(ALL) NOPASSWD:ALL' | sudo tee /etc/sudoers.d/vagrant
      SHELL
    end
  
    # Define VM 3
    config.vm.define "vm3" do |vm3|
      vm3.vm.box = "ubuntu/focal64"
      vm3.vm.hostname = "VM3"
      vm3.vm.network "private_network", ip: "192.168.56.103"
      vm3.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = 2
      end
      vm3.vm.provision "shell", inline: <<-SHELL
        sudo apt-get update
        sudo apt-get upgrade -y
        echo 'vagrant ALL=(ALL) NOPASSWD:ALL' | sudo tee /etc/sudoers.d/vagrant
      SHELL
    end
  end
  
