vagrant-kvmhost
===============

local development kvm/libvirtd server with Vagrant

### requirements

* Vagrant
* vmware fusion
* vagrant-vmware-fusion plugin

### run

``` shell
$ vagrant up
$ vagrant ssh -c "ip a"
```

#### connect

if your VM's IPv4 address is `192.168.1.10`, you can connect to `qemu+tcp://192.168.1.10/system` with libvirt.
