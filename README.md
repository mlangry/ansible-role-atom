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
atom_packages : []
````

Dependencies
------------

None

Example Playbook
----------------

````yaml
    - hosts: all
      roles:
        - { role: mlangry.atom, atom_ver: 1.7.3 }
````


````yaml
    - hosts: all
      roles:
        - role: mlangry.atom
          atom_packages:
            - minimap
            - { name: atom-beautify, state=present }
````

License
-------

MIT
