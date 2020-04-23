ansible-role-jobber [![Build Status](https://travis-ci.org/danihodovic/ansible-role-jobber.svg?branch=master)](https://travis-ci.org/danihodovic/ansible-role-jobber)
=========

An Ansible role that installs Jobber on debian based architecture.

https://dshearer.github.io/jobber

Requirements
------------

Role Variables
--------------

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: danihodovic.jobber
      vars:
        jobber_configs:
          root:
            version: 1.4
            jobs:
              root_job:
                cmd: echo hello root
                time: 0 0 12
```
Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: danihodovic.jobber, x: 42 }

License
-------

MIT

Author Information
------------------

Dani Hodovic @danihodovic https://hodovi.ch
