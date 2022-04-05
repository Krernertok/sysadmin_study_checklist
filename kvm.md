# KVM

## Getting started

### To use `qemu:///system` by default

	1. Copy `/var/lib/libvirt/libvirt.conf` under `~/.config/libvirt/` and uncomment the `uri_defaul` line.
	2. Uncomment the following lines from `/etc/libvirt/libvirtd.conf`:
		- `unix_sock_group`
		- `unix_sock_ro_perms`
		- `unix_sock_rw_perms`
	3. Add the user to the group used in `unix_sock_group` (most likely "libvirt") and log that user in again (for the changes to apply).


### Creating a VM using `virt-install`

		virt-install \
			--name test-vm \
			--ram 1024 \
			--vcpus 2 \
			--os-type linux \
			--os-variant generic \
			--hvm \
			--console pty,target_type=serial \
			--cdrom ~/linux-iso/ubuntu-20.04.4-live-server-amd64.iso \
			--disk path=/var/lib/libvirt/images/test-ubuntu.qcow2,size=10

### Removing a VM

		virsh destroy test-vm; virsh undefine test-vm

