swygue-smartd
=============

Installs and configures smartd with a notification script for emailing SMART disk errors.

This role was tested on Fedora 27 only.

https://github.com/CSCfi/ansible-role-smartd

Requirements
------------

System is configured to send emails. The notification script uses /usr/bin/mail.

Role Variables
--------------

See defaults/main.yml

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
- hosts: servers
  roles:
     - { role: swygue-smartd }
```

License
-------

MIT

Author Information
------------------

Inspiration taken from https://github.com/CSCfi/ansible-role-smartd
