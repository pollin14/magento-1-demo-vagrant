## Requirements

You need to install

* Ansible 2.*
* Vagrant from its website
* git

## Installation

To run 

```
vagrant up
```

## Ansible notes

To debug a variable you can, 

## Useful tips

### Resize disk

#### Change format from vmdk to vdi

```
cd ~/VirtualBox\ VMs/my-vm-name \
VBoxManage clonehd "box-disk1.vmdk" "cloned.vdi" --format vdi \
VBoxManage modifyhd "cloned.vdi" --resize 90200
```

Using the VB UI change the disk box-disk1 to cloned.vdi.

That is all.

## Issues

If you are using rsync or FTP it is necessary reload the VM to solve permission issues.