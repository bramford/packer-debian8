Packer templates for Debian 8 (jessie)
--------------------------------------
 
## Overview
 
Fully automated installation of Debain 8; powered by Packer, Debian Preseed and Ansible

- [Packer](https://www.packer.io/intro/index.html)
- [Ansible](http://docs.ansible.com/ansible/index.html)
- [Debian Preseed](https://wiki.debian.org/DebianInstaller/Preseed)

### Dependencies
 
 - Packer 0.10.2+ (from https://www.packer.io/downloads.html)
 
-## Build
## qemu-kvm

### Install Dependencies

    apt-get install qemu-kvm

### Build
 
    packer build packer-debain8-qemu-kvm.json -var 'local_domain=lan.mydomain.com'
 
### Output
 
Resulting image will be stored in `./output/`.
