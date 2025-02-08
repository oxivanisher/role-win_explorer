win_explorer
============
[![Ansible Lint](https://github.com/oxivanisher/role-win_explorer/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/oxivanisher/role-win_explorer/actions/workflows/ansible-lint.yml)

Configure explorer related settings:
* Show file extensions
* Disable ribbon menu
* Disable new right-click context menu
* Disable "Edit in Notepad" in right-click context menu
* Removes the "Onedrive Personal" in left pane

Requirements
------------

This role is built to be used with Ansible oder SSH on Windows.

Role Variables
--------------

| Name                               | Comment                        | Default value |
|------------------------------------|--------------------------------|---------------|
| win_explorer_users                 | List of users to be configured | `[Default]`   |
| win_explorer_also_for_ansible_user | Also configure `ansible_user`  | `true`        |

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
