## Requirements

You need to install

* Ansible 2.*
* Vagrant from its website
* git

## Installation



## Notes

If you want to install a database from production securely the size of the virtual disk
 will not enough. So you need to resize with the following commands
 
```
cd ~/VirtualBox\ VMs/elpalaciodehierro/ &&\
VBoxManage clonehd "box-disk1.vmdk" "cloned.vdi" --format vdi &&\
VBoxManage modifyhd "cloned.vdi" --resize 100200
```

Then you need to open the UI of virtual box and assign the recient cloned disk.
after this, you can work with vagrant normally.