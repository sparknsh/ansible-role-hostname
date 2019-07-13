# Ansible Role: Hostname

#### Version: 1.0.1

[![](https://img.shields.io/badge/role-sparknsh.hostname-blue.svg)](https://galaxy.ansible.com/sparknsh/hostname)

Development of this project is managed in a private repository then pushed out to [GitLab](https://gitlab.com/sparknsh/ansible-role-hostname) and [GitHub](https://github.com/sparknsh/ansible-role-hostname) when we have a new version for you. If you have any issues please contact [sparknsh](https://www.sparknsh.com/contact?type=issue&name=ansible-role-hostname)

## Role Variables

```yaml
hostname__fqdn: "{{ inventory_hostname }}"
hostname__hosts: []
```

#### Example

```yaml
hostname__fqdn: "{{ inventory_hostname }}"
hostname__hosts:
  myhost.com: 192.168.1.1
  yourhost.com: 192.168.1.2
```

## Example Playbook

```yaml
- hosts: all
  vars_files:
    - vars/main.yml
  roles:
     - { role: sparknsh.hostname }
```

## License

MIT

## Author Information

This role was created in 2019 by [sparknsh](https://www.sparknsh.com) at [Rebel Media, Inc.](https://www.rebelmedia.io/)
