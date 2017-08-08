csec-ansible-pb
====================

This projet contains the infrastructure configuration layer of CSEC servers.
In these playbooks, we configure:

- users
- ssh public keys
- sudoser
- dns
- hosts file
- ntp
- network
- packet managers
- basic packages
- updates
- logs
- sssd
- default parameters
- default system tunning
- system certificates

All roles should be stored on individual repositories on github and used as
galaxy roles. Please also specify versions.

### Installation

Install role dependencies :

    ansible-galaxy install -r requirements.yml


Update role dependencies:

    ansible-galaxy install -r requirements.yml --force


### Usage

    ansible-playbook playbook.yml -D


`playbook.yml` is the main playbook.

`-D` to display diff

`-C` to use check mode and don't do anything (optional)

`-u` to specify remote user (optional)

`-K` to ask for ssh password (optional)

`-k` to ask for "become" (sudo) password (optional)


