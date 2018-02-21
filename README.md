swygue-smartd
=============

Installs and configures smartd with a notification script for emailing SMART disk errors.

About the notification
----------------------

```
DEVICESCAN -a -o on -S on -n standby,q -s (S/../.././02|L/../../6/03) -W 4,35,40 -m <email> -M exec /usr/local/bin/smartdnotify
```

This does:
- A short test every day from 2 a.m..
- A long test every Saturday at 3 a.m..

Then sends an email when SMART detects an error.

This role was tested on Fedora 27 only.

https://github.com/flyemsafe/swygue-smartd

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
