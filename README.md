ansible-role-jobber [![Build Status](https://travis-ci.org/danihodovic/ansible-role-jobber.svg?branch=master)](https://travis-ci.org/danihodovic/ansible-role-jobber)
=========

An Ansible role that installs Jobber on debian based architecture.

https://dshearer.github.io/jobber

Requirements
------------

- jmespath (`pip install jmespath`) on the controller machine

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: ansible-role-jobber
      vars:
        jobber_configs:
          root:
            version: 1.4
            jobs:
              root_job:
                cmd: echo hello root
                time: 0 0 12

          dani:
            version: 1.4
            jobs:
              other_job:
                cmd: echo hello dani
                time: 0 0 12
```

License
-------

MIT

Author Information
------------------

Dani Hodovic @danihodovic https://hodovi.ch
