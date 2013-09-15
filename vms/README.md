# VMs

This directory contains [Packer](http://www.packer.io/) templates and required
resources to build from scratch the VMs used for development or testing.

Thanks to Packer, these templates can also be used to create images for
different providers, like AMI for Amazon EC2 or Digital Ocean images.

Please refer to Packer documentation on how to modify those.

The code here was stolen from [emilisto/packer.io-playground](https://github.com/emilisto/packer.io-playground) and tailored for the needs of my project, which is running with
VirtualBox and nothing else.

All credits goes to the original author.

## Building

Easy, just:

    $ packer build ubuntu-rarin64.json

And go grab some coffee.

## Installing it

Now that you have your box, it will be named `packer_virtualbox_virtualbox.box`.
Simply install it as `raring64-packer` box into vagrant:

    $ vagrant box add raring64-packer packer_virtualbox_virtualbox.box

And done.
