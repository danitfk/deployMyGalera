deployMyGalera - MariaDB Galera Cluster with Ansible
=========

An Ansible playbook to privision MariaDB Galera cluster on Ubuntu/Debian distros.

Requirements
------------

- Python installed -> ` apt install python -y `
- Proper Internet acess to install packages and repositories
- An admin access (sudo) to the server.

Role Variables
--------------

All variables can be found in `galeraCluster/default/main.yml` file.
There is some configuartion like `mariadb_version` , `innodb_buffer_pool_size` , available for adjustment.


Example Playbook
----------------

You can use this example to run playbook:
```
---
- hosts: galera
  become: true
  roles:
  - galeraCluster
```
It can be found with `main.yml.example` filename.

License
-------

The Unlicensed

