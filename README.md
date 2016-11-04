[![Build Status](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nhc-scripts.svg?branch=master)](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nhc-scripts)
ansible-role-nhc-scripts
=========

get_url or copy custom NHC ( Node Health Checker https://github.com/mej/nhc ) plugins 

This role is _not_ a distribution point of NHC checks - store them where you run ansible or on a web server, or even better package them in RPMs and don't use this role at all :)

Requirements
------------

 - ansible-role-nhc: https://github.com/CSC-IT-Center-for-Science/ansible-role-nhc
  - or at least https://github.com/mej/nhc

Role Variables
--------------

nhc_scripts_copy:
 - 

nhc_scripts_geturl:
 - url, dest

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible-role-nhc-scripts }
         - { role: ansible-role-nhc }

License
-------

MIT

Author Information
------------------
