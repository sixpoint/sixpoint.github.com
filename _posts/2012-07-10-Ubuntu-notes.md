---
layout: post
title: "Ubuntu notes"
description: "Ubuntu notes"
category: notes
tags: [ubuntu]
---
{% include JB/setup %}

- `export http_proxy=http://127.0.0.1:8087/` # Using goagent proxy for shell
- using pip install with proxy:  `pip --proxy "http://127.0.0.1:8087" install Fabric==1.4.0`

- `mount -t vboxsf vboxsf_in_windows /mnt/shared` # let it auto, insert it into `/etc/init.d/rcs`
Change hosts in /etc/host
- change to the root: `sudo su`
- `sudo netstat -tulpn| grep :80`
- `sudo chown -R username:www-data /home/dir`
- `sudo chmod -R g+w /home/dir`
- `dig -t TXT _netblocks.google.com @ns1.google.com` Check netblocks
- `top`
- `ssh -C2qTnN -D 8080 username@remote_machine.com`


Using vagrant
=============
- Download boxes from hrer [Available boxes](https://github.com/mitchellh/vagrant/wiki/Available-Vagrant-Boxes)
- `the box 'base' could not be found vagrant` error
- Just using: `vagrant box add base lucid32.box`  
- `vagrant box list`
- `vagrant init lucid32`
- `vagrant up`

Centos/Cpanel/VPS
===========
- [Set up mail MX record](http://www.webhostgear.com/272.html)
