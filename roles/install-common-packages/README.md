Install common packages
=========

This role install the last version of a list of packages.

Requirements
------------

None.

Role Variables
--------------

The list of packages to be installed.

Example Playbook
----------------

    - hosts: servers
      become: true
      roles:
         - install-common-packages

License
-------

Free

Author Information
------------------

Gabriel Richter <<gabrielrih@gmail.com>>