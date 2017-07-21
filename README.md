# hashicorp-binary

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-hashicorp-binary.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-hashicorp-binary)

ansible role to install Hashicorp's binary.

https://galaxy.ansible.com/suzuki-shunsuke/hashicorp-binary/

## Requirements

Nothing.

## Role Variables

name | required | default | description
--- | --- | --- | ---
hashicorp_binary_name | yes | | https://releases.hashicorp.com/
hashicorp_binary_arch: | yes | | linux_amd64, etc
hashicorp_binary_version | yes | | installed binary version
hashicorp_binary_lib_dir | no | /usr/local/lib | The install path. This directory is generated if it doesn't exist
hashicorp_binary_bin_dir | no | /usr/local/bin | The install path. This directory is generated if it doesn't exist

## Dependencies

Nothing.

## Example Playbook

```yaml
- hosts: servers
  roles:
  - role: suzuki-shunsuke.hashicorp-binary
    hashicorp_binary_name: terraform
    hashicorp_binary_arch: linux_amd64
    hashicorp_binary_version: 0.9.11
    hashicorp_binary_lib_dir: /usr/local/lib
    hashicorp_binary_bin_dir: /usr/local/bin
    become: yes
  - role: suzuki-shunsuke.hashicorp-binary
    hashicorp_binary_name: consul
    hashicorp_binary_arch: linux_amd64
    hashicorp_binary_version: 0.8.4
    hashicorp_binary_lib_dir: "{{ansible_env.HOME}}/lib"
    hashicorp_binary_bin_dir: "{{ansible_env.HOME}}/bin"
```

## Change Log

See [CHANGELOG.md](CHANGELOG.md).

## License

[MIT](LICENSE)
