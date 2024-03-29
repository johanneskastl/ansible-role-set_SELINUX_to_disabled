![Ansible Lint](https://github.com/johanneskastl/ansible-role-set_SELINUX_to_disabled/workflows/Ansible%20Lint/badge.svg)

set_SELINUX_to_disabled
=========

Set SELINUX to disabled, reboot the machine and check the status after the reboot.

Requirements
------------

None.

Role Variables
--------------

- `selinux_policy`: SELINUX policy, defaults to `targeted`.

Dependencies
------------

This requires the [`johanneskastl.reboot` role](https://github.com/johanneskastl/ansible-role-reboot) to reboot the nodes in case of changes.

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: 'johanneskastl.set_SELINUX_to_disabled'

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
