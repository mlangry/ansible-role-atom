mlangry.atom[![Build Status](https://travis-ci.org/mlangry/ansible-role-atom.svg?branch=master)](https://travis-ci.org/mlangry/ansible-role-atom)
=========

Support for Atom editor via Ansible.

Requirements
------------

Fedora:

  python-dnf

Role Variables
--------------

````yaml
atom_ver : '1.8.0'
atom_mirror : 'https://github.com/atom/atom/releases/download'
atom_deb_platform : 'amd64'
atom_rpm_platform : 'x86_64'
````

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables
 passed in as parameters) is always nice for users too:

````yaml
    - hosts: all
      roles:
        - { role: mlangry.atom, atom_ver: 1.7.3 }
````

License
-------

MIT
