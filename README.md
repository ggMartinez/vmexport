vmexport
========

KVM Virtual Machine Export Script.

vmexport is a bash script that allow to migrate a Virtual Machine from one KVM Server to another, keeping all its confis, HDDs, NICs, etc.

It uses a few virsh commands to get the configs and the HDD file, and then, with ssh, copy the files to the destination server, and then register the VM to it.









