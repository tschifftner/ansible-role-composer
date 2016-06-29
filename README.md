# Ansible Role: Install Composer

[![Build Status](https://travis-ci.org/tschifftner/ansible-role-composer.svg)](https://travis-ci.org/tschifftner/ansible-role-composer)

Installs composer on Debian/Ubuntu linux servers. Installs cronjob to sel-update

## Requirements

PHP must be installed prior to running this role!
ansible 2.0+

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
## Supported OS
Ansible          | Debian Jessie    | Ubuntu 14.04    | Ubuntu 12.04
:--------------: | :--------------: | :-------------: | :-------------: 
2.0              | Yes              | Yes             | Yes
2.1              | Yes              | Yes             | Yes


## License

MIT / BSD

## Author Information

 - Tobias Schifftner, @tschifftner