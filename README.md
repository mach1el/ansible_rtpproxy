# Ansible Role for RTPengine
![Version](https://img.shields.io/github/v/release/mach1el/ansible-role-rtpproxy?color=blue&style=plastic) ![License](https://img.shields.io/github/license/mach1el/ansible-role-rtpproxy?color=grey&style=plastic)

Auto build,deploy rtpproxy with ansible.

## Role variables
See [`default/main.yml`](https://github.com/mach1el/ansible-role-rtpproxy/blob/master/defaults/main.yml)

## Role pathes

    ├── defaults
    │   └── main.yml
    ├── handlers
    │   └── main.yml
    ├── tasks
    │   ├── configure.yml
    │   ├── main.yml
    │   ├── setup_bcg.yml
    │   ├── setup_debian.yml
    │   └── setup_rtpengine.yml
    └── templates
        ├── rtpengine.conf.j2
        └── rtpengine-recording.conf.j2

## Example playbook

    ---
    - name: Building rtpengine for local server
      hosts: local_server
      become: true
     
      roles: - '../ansible-role-rtpproxy'
