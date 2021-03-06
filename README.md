Ansible Hostname Role
=====================

An ansible role for installing and configuring the hostname.
This role will only set the hostname and will not edit the /etc/hosts file! Use the hosts role to update your hosts file.

Role Variables
--------------

```yaml
hostname_custom_name: set a custom hostname. If none specified, the short inventory hostname will be used as default.
```

Example Playbook
-------------------------

```yaml
- hosts: servers
  roles:
     - { role: MichaelRigart.hostname, hostname_custom_name: custom_name, become: true }
```

License
-------

GPLv3

Author Information
------------------

Michaël Rigart <michael@netronix.be>
