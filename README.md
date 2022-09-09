Ansible-Docker Role
=========

Simple Ansible role for deploying Docker CE on your Linux machine

Requirements
------------

- Ansible 2.7 or higher
- Linux server

Role Variables
--------------

- `docker_version` # version of docker main packages
- `docker_ce_cli_version` # version of docker main packages
- `containerd_version` # version of CRI Containerd to be installed
- `docker_apt_repository` # docker's url of repository
- `apt_gpg_key` # apt_gpg_key's version to be taken from docker.com

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      become: yes
      vars_file:
       - vars/main.yml
      roles:
         - { role: ansible-docker }
```
