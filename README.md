ansible-role-nginx
=========

Currently only tested and compatible  with CentOS 7.
Installs nginx and configures a user defined nginx config and vhost file.

Requirements
------------

Knowledge of using Ansible is required.

Role Variables
--------------

Users are to manage nginx configuration.

You will need to overried variables where configuration
are found in your playbook.

* `nginx_config_file`: the nginx.conf file
* `nginx_confd_dir`:  directory w/ vhost files
* `nginx_ssl_dir`:  directory w/ ssl certs files

Dependencies
------------

None

Example Playbook
----------------

```
- hosts: servers
  roles:
     - { role: xyzrbt.nginx }
```

License
-------

GPLv2

Author Information
------------------

github.com/xyzrbt
