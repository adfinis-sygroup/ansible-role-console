# ROLE CONSOLE

[![GitHub](https://img.shields.io/github/license/adfinis-sygroup/ansible-role-console.svg?style=flat-square)](https://github.com/adfinis-sygroup/ansible-role-console/blob/master/LICENSE)
[![Travis (.org)](https://img.shields.io/travis/adfinis-sygroup/ansible-role-console.svg?style=flat-square)](https://travis-ci.org/adfinis-sygroup/ansible-role-console)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-adfinis--sygroup.console-660198.svg?style=flat-square)](https://galaxy.ansible.com/adfinis-sygroup/console)

This role configures and manages various console related topics:

* Set of handy default tools to have available on the system for daily business
* VIM, git and shell (bash) configuration

## Requirements

This role has no additional requirements.

## Role Variables

The following defaults variables can be configured:

``` yaml
# Set backupcopy default to no
console_vim_backupcopy: False

# disable mouse support (Only Debian)
console_vim_mouse_disable: False
```

For a list OS related variables that usually don't need to be customized have a
look at the vars/ directory.

## Dependencies

This role has no additional dependencies.

## Example Playbook

Below example shows how the role can be integrated into a playbook using
external vars:

``` yaml
- hosts: servers
  roles:
    - { role: adfinis-sygroup.console }
```

## License

[GPL-3.0](https://github.com/adfinis-sygroup/ansible-role-console/blob/master/LICENSE)

## Author Information

console role was written by:

-   Adfinis SyGroup AG \| [Website](https://www.adfinis-sygroup.ch/) \|
    [Twitter](https://twitter.com/adfinissygroup) \|
    [GitHub](https://github.com/adfinis-sygroup)
