## Ansible Role: Generate SSL Certificate from Lets Encrypt through CNAME ( Route53 )

[![Build Status](https://travis-ci.org/meabed/ansible-role-lets-encrypt-cname.svg?branch=master)](https://travis-ci.org/meabed/ansible-role-lets-encrypt-cname)
[![Platforms](https://img.shields.io/badge/platforms-debian%20/%20ubuntu%20/%20redhat%20/%20freebsd-blue.svg?style=flat)](#)
[![@Meabed](https://img.shields.io/badge/twitter-@meabed-179BD7.svg?style=flat-squares)](https://twitter.com/meabed)
[![Authoer Blog](https://img.shields.io/badge/Author-blog-green.svg?style=flat-square)](https://meabed.com)

## Description

An Ansible Role to generate lets encrypt ssl certificate with domain hosted on Route53 using CNAME Strategy
                   

## References

* [docs.ansible.com](https://docs.ansible.com/)

## Variables

### defaults/main.yml

* [defaults/main.yml](defaults/main.yml) contains all of the required variables.

### example playbook

* [test_debian.yml](tests/docker/test_debian.yml) may contain an example entry.

### For Testing [Docker](https://www.docker.com/)

Test with Docker for an easier experience
- to test specific OS use one of those docker images from https://hub.docker.com/u/geerlingguy/

```shell
$ cd roles/lte-acme-cname
$ docker run --privileged -u 0 -v ~/Workspace:/Workspace -it geerlingguy/docker-debian8-ansible /bin/bash
$ cd /Workspace
$ ansible-playbook tests/docker/test_debian.yml -vvvv -e lte_access_key=__AWS_ACCESS_KEY__ -e lte_secret_key=__AWS_SECRET_KEY__

```

### OS's tested with Docker

pass, fail, untested

| Distribution | Results  |
| ------------ | -------- |
| precise      | pass ✅ |
| trusty       | pass ✅ |
| xenial       | pass ✅ |
| bionic       | pass ✅ |
| CentOS 6     | pass ✅ |
| CentOS 7     | pass ✅ |

## Roadmap

* [ROADMAP.md](ROADMAP.md)

## Authors and License
- [Mohamed Meabed](https://meabed.com/) | [e-mail](mailto:mo@meabed.com)
- License: [MIT](LICENSE)
