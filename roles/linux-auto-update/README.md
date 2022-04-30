Linux Auto Update
=========

This role is reponsible for configure a auto update in Linux system. This role works on Debian family and run apt update, upgrade, dist-upgrade and more.

Requirements
------------

The OS family must be Debian.

Role Variables
--------------

The most important variable in this role is the version of the package which contain all the logic to run the update.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      become: true
      roles:
         - linux-auto-update

License
-------

Free

Author Information
------------------

Gabriel Richter <gabrielrih@gmail.com>
