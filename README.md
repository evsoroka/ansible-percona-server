# Role Name
=========

Installs Percona MySQL Server on Debian/Ubuntu Linux system. Tested on Ubuntu 18.04, but should work on all versions

## Requirements
------------

None

## Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    db_version: 5.7

Which package version to install.

  mysql_root_password: 756fgRTsf!efsfTY

Specify the root password.

## Dependencies
------------

None

## Example Playbook
----------------

 - hosts: servers
   remote_user: root
   become: yes
   become_method: sudo
   roles:
    - ansible-percona-server
   vars:
    - db_version: 5.7
    - 

## License
-------

BSD

## Author Information
------------------

This role was created by Evgenios Soroka
