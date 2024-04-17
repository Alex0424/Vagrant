# Vagrant For Windows

https://youtu.be/czMCO1w-xQU?list=PLhW3qG5bs-L9S272lwi9encQOL9nMOnRa

https://www.youtube.com/watch?v=a6W1hF9CgDQ

download vagrant: https://developer.hashicorp.com/vagrant/install#windows

chose a box: https://app.vagrantup.com/boxes/search

### PowerShell (replace "centos/8" with your box.)

```
mkdir my_vagrant_file
vagrant init generic/centos9s
notepad .\Vagrantfile
```

### Vagrantfile:

```
Vagrant.configure("2") do |config|
  config.vm.hostname = "vm10"
  config.vm.box = "ubuntu/trusty64"
 config.vm.provision "shell", inline: <<-SHELL
   apt-get update
   apt-get install -y apache2
 SHELL
end
```

### PowerShell
```
vagrant up
vagrant ssh
```
