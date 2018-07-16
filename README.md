# Ansible Role: Install Composer

[![Build Status](https://travis-ci.org/tschifftner/ansible-role-composer.svg?branch=master)](https://travis-ci.org/tschifftner/ansible-role-composer)

Installs composer on Debian/Ubuntu linux servers. Installs cronjob to sel-update

## Requirements

PHP must be installed prior to running this role!

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
composer_selfupdate: true
composer_selfupdate_specialtime: weekly
```

## Dependencies

None.

## Installation

```
$ ansible-galaxy install tschifftner.composer
```

## Example Playbook

    - hosts: server
      roles:
        - { role: tschifftner.composer }

## Supported OS

 - Debian 9 (Stretch)
 - Debian 8 (Jessie)
 - Ubuntu 18.04 (Bionic Beaver)
 - Ubuntu 16.04 (Xenial Xerus)
 
## Required ansible version

Ansible 2.5+

## License

[MIT License](http://choosealicense.com/licenses/mit/)

## Author Information

 - [Tobias Schifftner](https://twitter.com/tschifftner), [ambimax® GmbH](https://www.ambimax.de)