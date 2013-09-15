# learning ansible

This is my attempt to understand concepts and structure of [Ansible](https://github.com/ansible/ansible)
and at the same time be able to create something useful and maintainable, at
least for me.

The idea is be able to provision individual web servers to run my Ruby
applications or cluster with specific roles.

Keep reading if you're interested in the details.

## Requirements

To work on this project you will [Vagrant](http://www.vagrantup.com/) and, of
course, [Ansible](https://github.com/ansible/ansible). Please refer to the
[Getting Started](http://www.ansibleworks.com/docs/gettingstarted.html)
documentation on how to obtain Ansible for your platform.

At this time, the following versions were used

- Vagrant 1.3.1 (which supports Ansible)
- Ansible 1.3.0
- Ubuntu 13.04 VM (built with [Packer](http://www.packer.io/))
