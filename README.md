Role Name
=========

Install the targeted version of ovh kernel in your VPS or dedicated server.

This has been tested only on debian, but should work with mosts of distros.

Requirements
------------

none

Role Variables
--------------

```YAML
- ovh_kernel_image_baseurl: 'ftp://ftp.ovh.net/made-in-ovh/bzImage/latest-production'
- ovh_kernel_image_version: '3.14.32'
- ovh_kernel_image_flavor: 'xxxx-std-ipv6-64'
- ovh_kernel_image_systemmap_basename: 'System.map'
- ovh_kernel_image_bzimage_basename: 'bzImage'
- ovh_kernel_image_config_basename: 'config'
```

Dependencies
------------

none

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: webofmars.ovh-kernel }

License
-------

BSD

Author Information
------------------

[webofmars](https://webofmars.com) 2017
