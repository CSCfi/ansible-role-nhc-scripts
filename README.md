[![Build Status](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nhc-scripts.svg?branch=master)](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nhc-scripts)
ansible-role-nhc-scripts
=========

get_url or copy custom NHC ( Node Health Checker https://github.com/mej/nhc ) plugins 

This role is _not_ a distribution point of NHC checks - store them where you run ansible or on a web server, or even better package them in RPMs and don't use this role at all :)

**nhc_remote_url_checks** can be used with ansible-pull

**nhc_local_checks** can be used with ansible-playbook (push mode) to copy checks

Requirements
------------

 - ansible-role-nhc: https://github.com/CSC-IT-Center-for-Science/ansible-role-nhc
  - or at least https://github.com/mej/nhc

Role Variables
--------------

Example:
<pre>
nhc_remote_url_scripts:
 - { url: "http://url1/nhc_script_1", name: "nhc_script_1", scriptsum: "7e39171be1095b3c6a35c9649e3d5e73bcf76a3647b99fd7a205248a35d6a6f9" }
nhc_local_scripts:
 - { path: "files/nhc_script_2", name: "nhc_script_2" }
</pre>

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
