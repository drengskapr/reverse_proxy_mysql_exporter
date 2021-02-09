reverse_proxy_mysql_exporter
=========

Installs and sets up nginx as reverse proxy for mysqld_exporter's `/metrics` endpoint with basic auth. 

Requirements
------------

Debian 10

Role Variables
--------------

`basic_auth_name` basic auth username.

`basic_auth_password` basic auth password.


Example Playbook
----------------

```
- name: Setting up reverse_proxy
  hosts: all
  remote_user: root
  roles:
    - reverse_proxy_mysql_exporter
  vars:
    basic_auth_name: user
    basic_auth_password: password
```

License
-------

BSD

