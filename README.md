# What is Vagrant?

It is a VM automation tool wich uses Hypervisors to manage vm's on our host-machine.

A Vagrant box is essentially a pre-packaged virtual machine image
- Box Size: 500 MB – 2 GB
- They are lighter than manually managing full VM snapshots
  - no GUI, minimal services
- They are heavier compared to containers because they run a full guest operating system on a hypervisor.

## [Download Vagrant](https://developer.hashicorp.com/vagrant/install)

## Start one Vagran VM machine

1. Find a ['Vagrant Box' from HashiCorp](https://portal.cloud.hashicorp.com/vagrant/discover)

2. Initialize the box:

```shell
vagrant init <box-name>
```

3. Start the box:

```shell
vagrant up
```

4. SSH in to the box:

```shell
vagrant ssh
```
