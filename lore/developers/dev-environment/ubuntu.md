---
name: ubuntu
layout: default
---

# Instructions for Ubuntu

## Table of Contents

* [Python Tools](#python-tools)
* [Virtualization Tools](#virtualization-tools)

## Python Tools

Run the following to install most of the needed packages:

```shell
$ sudo apt-get install build-essential libssl-dev libffi-dev python-dev python-pip python-software-properties
```

Install ansible, setuptools, virtualenv and virtualenvwrapper:

```shell
$ sudo pip install ansible setuptools virtualenv virtualenvwrapper
```

Add the following to your `~/.bashrc`:

```shell
export WORKON_HOME=~/.virtualenvs
. /usr/local/bin/virtualenvwrapper.sh
```

Activate virtualenvwrapper:

```shell
$ source ~/.bashrc
```

## Virtualization Tools

Install [VirtualBox](https://www.virtualbox.org) and [Vagrant](https://www.vagrantup.com) for running local virtual machines:

```shell
$ sudo apt-get install vagrant virtualbox
```

Install [vagrant-hostmanager](https://github.com/devopsgroup-io/vagrant-hostmanager), and [vagrant-triggers](https://github.com/emyl/vagrant-triggers):

```shell
$ vagrant plugin install vagrant-hostmanager vagrant-triggers
```
