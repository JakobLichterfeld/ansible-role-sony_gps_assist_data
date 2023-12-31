# Ansible Role: Sony-GPS-Assist-Data

[![CI](https://github.com/JakobLichterfeld/ansible-role-sony_gps_assist_data/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/JakobLichterfeld/ansible-role-sony_gps_assist_data/actions/workflows/ci.yml)
[![Publish role on Ansible Galaxy](https://github.com/JakobLichterfeld/ansible-role-sony_gps_assist_data/actions/workflows/publish_role_on_ansible_galaxy.yml/badge.svg?branch=main)](https://github.com/JakobLichterfeld/ansible-role-sony_gps_assist_data/actions/workflows/publish_role_on_ansible_galaxy.yml)

Install Sony-GPS-Assist-Data Script via git checkout

- Install Dependencies
- Git checkout the Bash Script

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

| Name           | Default Value   | Description                        |
| -------------- | --------------- | -----------------------------------|
| `sony_gps_assist_data.repo` | "https://github.com/Zigazou/SonyGPSAssist.git" | Repo of Bash Script |
| `sony_gps_assist_data.dest` | "/home/{{ ansible_user }}/Downloads/sony_gps_assist_data" | Destination folder from which you want to run the script |

## Dependencies

None.

## Example Playbook

```yaml
---
- hosts: all
  gather_facts: true
  become: true

  roles:
    - role: jakoblichterfeld.sony_gps_assist_data

```

## License

MIT

## Author Information

This role was created in 2023 by [Jakob Lichterfeld](https://github.com/JakobLichterfeld).
