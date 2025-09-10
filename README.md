# What is Vagrant?

It is a VM automation tool wich uses Hypervisors to manage vm's on our host-machine.

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
