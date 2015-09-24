# Ansible provisioning for CollectiveAccess

[![Latest Version](https://img.shields.io/github/release/netsensei/ansible-collectiveaccess.svg?style=flat-square)](https://github.com/netsensei/ansible-collectiveaccess/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)

## Ansible provisioning for CollectiveAccess

This project provides [Ansible](http://www.ansible.com) provisinioning for easy/quick installation and configuration of a [CollectiveAccess](http://collectiveaccess.org/) instance.

### What is CollectiveAccess?

[CollectiveAccess](http://collectiveaccess.org/) is webbased software for describing all manner of things, and allows you to create catalogues that closely conform to your needs without custom programming.

### Requirements

You will need a working installation of [Vagrant](https://www.vagrantup.com/) and [Ansible](http://www.ansible.com) on your machine.

### What is in the box?

- Ubuntu Trusty Thar 14.04
- 512Mb RAM
- NGinX based
- PHP 5.6 with a few required extensions
- MySQL database

## Install

Clone this repository to your local machine (we assume you have a dedicated workspace folder at `~/Workspace` refer to `Vagrantfile` to change this to a destination of your choice.)

```bash
cd ~/Workspace
git clone https://github.com/netsensei/ansible-collectiveaccess
```

Also, clone the [Providence](https://github.com/collectiveaccess/providence) repository to your Workspace folder

```bash
git clone https://github.com/collectiveaccess/providence
```

Now, go back to the Ansible folder and start Vagrant. Ansible should automatically start provisioning the box with all the necessary dependencies for CollectiveAccess.

```bash
cd ~/Workspace/ansible-collectiveaccess
vagrant up
```

## Usage

Out of the box, NGinX listens on IP address `192.168.2.145`. Alternatively, you could create an entry in your `/etc/hosts` file that points to `collectiveaccess.local`.

Open up your browser and navigate to either the IP address or the local domain. First time, you will be welcomed by the Providence installer.

## Documentation

## Security

If you discover any security related, please email matthias@colada.be instead of using the issue tracker.

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
