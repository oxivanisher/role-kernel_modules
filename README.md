kernel_modules
==============
[![Ansible Lint](https://github.com/oxivanisher/role-kernel_modules/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/oxivanisher/role-kernel_modules/actions/workflows/ansible-lint.yml)

At the current state, this module only supports denylisting modules. The name of the role was choosen to possibly support module configurations in the future

This role does not automatically reboot the system to activate the changes.

As always: Use at your own risk!

Role Variables
--------------

| Name                    | Comment                                                          | Default value |
|-------------------------|------------------------------------------------------------------|---------------|
| kernel_modules_denylist | A list of modules to be denylist  (aka not loaded during boot) | `[]`          |

Example Playbook
----------------
```yaml
- name: Configure kernel modules
  hosts: clients
  roles:
    - role: oxivanisher.linux_base.kernel_modules
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_base](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_base/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_base).
