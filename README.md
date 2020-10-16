role_bi_hostname
=========

Sets the hostname and fqdn.

Requirements
------------

n.a.

Role Variables
--------------
The hostname is read from "inventory_hostname".

The default domain ending is read from "role_bi_hostname_default_domain".

The entries in /etc/hosts are generated from the content of the list "role_bi_hostname_etc_hosts_entries".

These are the defaults configured:

```
# defaults file for role_bi_hostname/
role_bi_hostname_default_domain: "localnet"
role_bi_hostname_etc_hosts_entries:
  "127.0.0.1": "localhost localhost.localdomain localhost4 localhost4.localdomain4"
  "::1": "localhost localhost.localdomain localhost6 localhost6.localdomain6"
```

Dependencies
------------

n.a.

Example Playbook
----------------

n.a.

License
-------

GNU Public License

Author Information
------------------

Melanie Desaive, m.desaive@mailbox.org
