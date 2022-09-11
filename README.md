# Ansible Role for RTPproxy
![License](https://img.shields.io/github/license/mach1el/ansible_rtpproxy?color=grey&style=plastic)

Auto build,deploy rtpproxy with ansible.

## Role variables
See [`default/main.yml`](https://github.com/mach1el/ansible_rtpproxy/blob/master/defaults/main.yml)

## Role pathes

```
├── defaults
│   └── main.yaml
├── handlers
│   └── main.yaml
├── LICENSE
├── README.md
├── tasks
│   ├── create_service.yaml
│   ├── main.yaml
│   ├── setup_bcg.yaml
│   ├── setup_debian.yaml
│   └── setup_rtpproxy.yaml
└── templates
    └── rtpproxy.service
```

## Example playbook

```
---
- name: Building rtpengine for local server
  hosts: all
  become: true
  roles: 
    - 'mach1el.ansible_rtpproxy'
```
