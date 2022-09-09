Ansible-Docker Role
=========

Simple Ansible role for deploying Docker CE on your Linux machine

Requirements
------------

- Ansible 2.7 or higher
- Linux server

Role Variables
--------------

- `docker_ce_cli_version`
- `containerd_version`
- `docker_apt_repository`
- `apt_gpg_key`

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      become: yes
      vars.file:
        vars/mail.yml
      roles:
         - { role: ansible-docker }
```
