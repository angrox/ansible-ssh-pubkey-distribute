MaibornWolff ssh-pubkey-distribute
=========

The `ssh-pubkey-distribute` role is supposed to run on a regular basis.

This role ensures that the following packages are present 
* TBD

This role ensure that the following is configured 
* TBD

**IMPORTANT** 
* TBD 

Requirements
------------

* Tested on Ubuntu 16.04 LTS
* SSH keys must be placed in the respective directories (see config defaults)  

Role Variables
--------------

* `sshkey_add_dir`: ssh keys that must be added
* `sshkey_remove_dir`: ssh keys that must be removed
* `ssh_keyfile_user`: Name of the account that will be able to login.

Dependencies
------------

None.

Example Playbook
----------------
**defaults**

    TBD


**Usage**

```
# Base packages and config for all hosts
# Every hosts receives updated, gets date config and ssh hardening
- hosts: all
  roles:
    - { role:  roles/devops/ssh-pubkey-distribute,  tags: ssh-keys }
```

Tests
-----

TBD

TODOs
=====
* TBD

Author Information
------------------

* Martin Zehetmayer, MaibornWolff GmbH
* Florian Maier, MaibornWolff GmbH