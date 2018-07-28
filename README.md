ansible-hardening
=================

This ansible-hardening role applies security hardening configurations from the **Center for Internet Security** Guide (**CIS**), it provides important security-related configurations to systems running the following distributions:

* Red Hat Enterprise
* Ubuntu 16.04


For more details, review the
[ansible-hardening documentation](http://docs.openstack.org/developer/ansible-hardening/).


How to run
------------

Add your hosts to /hosts file, uncomment the roles that you want to run in /main.yml file, then run the following command:

```shell
ansible-playbook -i hosts main.yml
```

Checklist file
------------

Customize the checklist file located in the root directory to chose the configurations to apply.
Example:
```
network:
  # IPV4
  disable_ip_forwarding: yes
  disable_packet_redirect: no
```

Requirements
------------

This role can be used with or without OpenStack-Ansible. It requires
Ansible 2.3 or later.

Authors
-------
BITAM Salim [github.com/soolidsnake](https://github.com/soolidsnake).

MALAOUI Sidahmed bilal [github.com/sidahmed-malaoui](https://github.com/sidahmed-malaoui).


License
-------

GNU General Public License v3.0
