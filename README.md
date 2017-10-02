# Ansible Role: EPICS Base

Installs EPICS Base on RHEL/CentOS.

## Requirements

- ansible >= 2.3

## Role Variables
Refer to each `defaults/main.yml` in detail.
```
epics_host_arch: linux-x86_64
epics_base_url: "https://www.aps.anl.gov/epics/download/base/baseR3.14.12.6.tar.gz"
epics_extensions_top_url: "https://www.aps.anl.gov/epics/download/extensions/extensionsTop_20120904.tar.gz"
epics_base_unarchived_name: "base-3.14.12.6"
epics_directory: "/opt/epics/R314"
epics_base_name: "{{ epics_directory }}/base"
epics_extensions_name: "{{ epics_directory }}/extensions"
epics_modules_name: "{{ epics_directory }}/modules"
```

## Dependencies

None.

## Example Playbook
```
- hosts: epics-base
  roles:
    - role: ansible-role-epics-base
```

## License

None.

## Author Information

This role was created by Shinya Sasaki.
