# Ansible Role: entr

[![Build Status](https://travis-ci.org/mtlynch/ansible-role-entr.svg?branch=master)](https://travis-ci.org/mtlynch/ansible-role-entr)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-entr-blue.svg?style=flat-square)](https://galaxy.ansible.com/mtlynch/entr)
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](LICENSE)

Installs [entr](http://eradman.com/entrproject/) to Ubuntu/Debian systems.

## Role Variables

Available variables are listed below, along with default values (see [defaults/main.yml](defaults/main.yml)):

The version of entr to install.

```yaml
entr_version: 4.2
```

The location of entr source:

```yaml
entr_dir: "/var/lib/entr"
```

## Dependencies

None

## Example Playbook

#### `example.yml`

```yaml
---
- hosts: all
  become: True
  become_method: sudo
  become_user: root
  roles:
    - role: mtlynch.entr
```

### Running Example Playbook

To run the example playbook, `example.yml` (above), run the following commands:

```shell
ansible-galaxy install mtlynch.entr
ansible-playbook example.yml
```

## License

MIT

## Author Information

This role was created in 2019 by [Michael Lynch](https://mtlynch.io).
