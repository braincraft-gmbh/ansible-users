Role Name
=========

This role provides a central approach to user managament, allowing for:

* Creating users
* Adding the groups the users belong to
* Managing SSH keys per user
* Adding per user sudo commands

Requirements
------------

None.

Role Variables
--------------

For this role to do anything, an array of users with properties should be passed over (it's empty by default).

```
default_key: keys/empty.pub
users: []
# users:
#   - name: h.simpson
#     groups:
#       - simpsons
#       - nuclearmeltdown
#     sudo:
#       - /usr/sbin/coremeltdown
#       - /usr/local/bin/servebeer --amount 6


```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: all
      roles:
         - bc.users

License
-------

GNU GPL v3

Author Information
------------------

Gualter Barbas Baptista <gualter@ecobytes.net>
