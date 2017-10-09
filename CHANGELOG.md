# Change Log

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

<a name="3.0.1"></a>
## [3.0.1](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/compare/v3.0.0...v3.0.1) (2017-10-09)


### Bug Fixes

* fix meta/main.yml ([2eb102d](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/commit/2eb102d))



<a name="3.0.0"></a>
# [3.0.0](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/compare/v2.0.2...v3.0.0) (2017-07-21)


### Features

* allow to create hashicorp_binary_bin_dir and hashicorp_binary_lib_dir ([a84865c](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/commit/a84865c))


### BREAKING CHANGES

* If the remote user does not have the write permission of `hashicorp_binary_bin_dir` and
`hashicorp_binary_lib_dir`, the role level become option is required.



<a name="2.0.2"></a>
## [2.0.2](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/compare/v2.0.1...v2.0.2) (2017-07-21)


### Bug Fixes

* failed to uninstall the already installed binary ([a0645d7](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/commit/a0645d7))



<a name="2.0.1"></a>
## [2.0.1](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/compare/v2.0.0...v2.0.1) (2017-07-17)



<a name="2.0.0"></a>
# [2.0.0](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/compare/1.0.1...v2.0.0) (2017-07-17)


### Features

* change how to install ([2312a74](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/commit/2312a74))


### BREAKING CHANGES

* remove the `hashicorp_binary_install_dir` variable.



<a name="1.0.1"></a>
## [1.0.1](https://github.com/suzuki-shunsuke/ansible-hashicorp-binary/compare/1.0.0...1.0.1) (2017-01-14)



<a name="1.0.0"></a>
# 1.0.0 (2017-01-14)
