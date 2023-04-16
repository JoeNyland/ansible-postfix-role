joenyland.postfix
=========================

[![CI](https://github.com/JoeNyland/ansible-postfix-role/actions/workflows/ci.yml/badge.svg)](https://github.com/JoeNyland/ansible-postfix-role/actions/workflows/ci.yml)

Installs and configures Postfix.

Requirements
------------

None.

Role Variables
--------------

### `postfix_service`

A hash describing the desired state for the `postfix` service

### `postfix_inet_interfaces`

Interfaces that Postfix should listen on.

### `postfix_inet_protocols`

IP protocols that Postfix should communicate on.

### `postfix_host_name`

Hostname of the Postfix host.

### `postfix_mail_name`

Mail name of the Postfix host.

### `postfix_destinations`

Domains and hostnames that Postfix should receive mail for.

### `postfix_aliases`

Aliases to be stored in `/etc/aliases`.

### `postfix_networks`

Network subnets which Postfix should listen on.

### `postfix_relay_host_sasl_username`

User name to use to authenicate with a relay host.

### `postfix_relay_host_sasl_password`

Password to use to authenicate with a relay host.

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: server
  roles:
    - postfix
```

License
-------

MIT

Author Information
------------------

⌨️ with ❤️ by [Joe Nyland](https://joe.nyland.io)
