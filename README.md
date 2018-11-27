### Description

A Vagrant project that creates a ```vagrant box``` configured as follow:

- Hostname : ```bananas3```

- ip address : ```192.168.56.56```

- Installed software : ```nginx```

- Port forwarding : ```forwarded_port", guest: 80, host: 8080```

### Installed softwares needed prior to using the project

- VirtualBox software installation : [link for VirtualBox](https://www.virtualbox.org/wiki/Downloads)

- Vagrant software installation : [link for Vagrant](https://www.vagrantup.com/docs/installation/)

### The repo is having following files

- File ```scripts/provision.sh``` - a script that installs ```nginx```

- File ```Vagrantfile``` : Has the configuration for vagrant, about what type of VM we want, once set, executing vagrant up will have our clean environment

### How to use the repo

- Clone this repo to your local machines : `git clone git@github.com:galindonkov/vagrant-projectA.git`
- Change to the currently added directory : `cd vagrant-projectA/`
- Execute `vagrant up` to build your local DEV environment
- Once the DEV env is created, login to created VM machine by : `vagrant ssh`
- Once you finish with the test type `exit` to leave the Vagrant-built virtual machine.
- Bear in mind that the Vm will remain running, so in case it is not needed anymore you can either shut down the running machine Vagrant is managing by `vagrant halt` or using `vagrant destroy` to stop the running machine and destroy all resources that were created during the machine creation process.
