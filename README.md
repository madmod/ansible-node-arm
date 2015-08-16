ansible-node-arm
================

Ansible role to install the latest version of Node.js on ARM devices like the Rasperry pi from [node-arm](http://node-arm.herokuapp.com/).

Requirements
------------

An ARM device you want to be 100% more awesome in 90% less time! :laughing:
Tested on Raspian but it should work on anything Debian based.

Role Variables
--------------

Node version can be set to anything avalible from [node-arm](http://node-arm.herokuapp.com/).

```yaml
node_version: 'latest'
```

For experimental builds use this:
```yaml
node_version: 'latest_experimental'
```

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - role: madmod.ansible-node-arm
           node_version: '0.12.7'
```

License
-------

MIT


