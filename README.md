win_explorer
============

Configure explorer related settings.

Requirements
------------

This role is built to be used with Ansible oder SSH on Windows.

Role Variables
--------------

| Name                | Comment                        | Default value                    |
|---------------------|--------------------------------|----------------------------------|
| win_explorer_users  | List of users to be configured | `[Default, "{{ ansible_user }}"]`|

Example Playbook
----------------
```yaml
- name: Configure the Windows Explorer
  hosts: windows
  roles:
    - role: oxivanisher.windows_desktop.win_explorer
```
License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.windows_desktop](https://galaxy.ansible.com/ui/repo/published/oxivanisher/windows_desktop/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-windows_desktop).
