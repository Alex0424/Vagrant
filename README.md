# Commands for Vagrant

```
$ vagrant init box-name       #initialize a Vagrantfile
$ vagrant up                  #power on the vm & run vagrantfile config
$ vagrant halt                #power off the vm
$ vagrant destroy             #remove the vm
$ vagrant ssh                 #ssh in to the mashine
$ vagrant reload              #reboot the vm & run vagrantfile config
$ vagrant status              #show status of the vm
$ vagrant global-status       #show status on all vm on your machine
$ vagrant global-status prune #remove any invalid entries from the list & show status on all vm on your machine
$ vagrant box list            #lists all the downloaded boxes
```

# Commands inside an Vagrant VM

```
$ sudo -i     # switch to root user
$ exit        # exit out of root user or VM
```
