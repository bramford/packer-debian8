Packer Templates: Debian 8 (jessie)
-----------------------------------

[![Build Status](https://travis-ci.org/bramford/packer-debian8.svg?branch=master)](https://travis-ci.org/bramford/packer-debian8)
 
Fully automated installation of debain 8, powered by:

- [Packer](https://www.packer.io/intro/index.html)
- [Ansible](http://docs.ansible.com/ansible/index.html)
- [Debian Preseed](https://wiki.debian.org/DebianInstaller/Preseed)

## Dependencies
 
 - Packer [0.10.2+](https://releases.hashicorp.com/packer/)

## Key Features

- Partitioning with LVM
- Enables persistent network names
- Enables serial console
- Uses ansible for provisioning
 
# qemu-kvm

## Install Host Dependencies

    apt-get install qemu-kvm

## Build
 
    packer build packer-debain8-qemu-kvm.json -var 'local_domain=lan.mydomain.com'
 
## Output
 
Output directory defaults to `./output/`, configurable with `-var 'output_parent_dir=/path'`
