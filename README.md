vmexport
========

KVM Virtual Machine Export Script.

vmexport is a bash script that allow to migrate a Virtual Machine from one KVM Server to another, keeping all its confis, HDDs, NICs, etc.

It uses a few virsh commands to get the configs and the HDD file, and then, via ssh, copy the files to the destination server, and then register the VM to the KVM instance running on it.


Requirments
...........

OpenSSH
KVM

The script is kinda simple, it doesn't need any external packages to work properly. It uses normal commands that are always aviable on a normal KVM installation.


SSH Keys
...........

Since the whole process of migrating a VM is done with SSH, if you want to avoid the ssh authentication every time you want to migrate a VM, you need to generate SSH keys and then copy it to the destination server.
