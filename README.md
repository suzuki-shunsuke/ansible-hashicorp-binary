hashicorp-binary
================

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-hashicorp-binary.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-hashicorp-binary)

Install hashicorp-binary on Linux.

https://galaxy.ansible.com/suzuki-shunsuke/hashicorp-binary/

Requirements
------------

* unzip

Role Variables
--------------

* hashicorp_binary_name: https://releases.hashicorp.com/
* hashicorp_binary_arch: linux_amd64, etc
* hashicorp_binary_version: The version.
* hashicorp_binary_install_dir: The install path. The default is /usr/local/bin

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - role: suzuki-shunsuke.hashicorp-binary
    hashicorp_binary_name: terraform
    hashicorp_binary_arch: linux_amd64
    hashicorp_binary_version: 0.8.4
    hashicorp_binary_install_dir: /usr/bin
```

License
-------

MIT
