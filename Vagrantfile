# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.

  # config.vm.network "forwarded_port", guest: 80, host: 8080
  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"
  # vb.gui = true

Vagrant.configure("2") do |config|

config.vm.define "vm0" do |vm0|
    vm0.vm.box = "generic/ubuntu2204"
    vm0.vm.network "private_network", ip: "192.168.56.130"
    vm0.vm.network "public_network", bridge: "enp4s0"

    vm0.vm.provider "virtualbox" do |vb|
      vb.cpus = 8
      vb.memory = "8192"

    config.vm.provision "shell", path: "add_ssh_key.sh"
    end
  end

  config.vm.define "vm1" do |vm1|
    config.vm.box = "generic/ubuntu2204"
    vm1.vm.network "private_network", ip: "192.168.56.140"
    vm1.vm.network "public_network", bridge: "enp4s0"

    vm1.vm.provider "virtualbox" do |vb|
      vb.cpus = 4
      vb.memory = "4096"

    config.vm.provision "shell", path: "add_ssh_key.sh"
    end
  end
end
