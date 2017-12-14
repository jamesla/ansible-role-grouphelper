# ansible-role-grouphelper

A small handy reusable role to add users to groups.

## Usage:

playbook.yml:
```
---
- hosts: localhost
  vars:
    group_helper:
      - { user: root, groups: ['group1', 'group2'] }
  roles:
    - ansible-role-grouphelper
```
requirements.yml:
```
- src: https://github.com/jamesla/ansible-role-grouphelper.git
  version: master
  name: ansible-role-grouphelper
```
