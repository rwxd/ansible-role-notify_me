# Ansible Role to install notify-me

With this ansible role [notify-me](https://github.com/rwxd/notify-me/) can be installed to the target system.

The correct binary for the operating system & architecture is automatically choosen.

## Usage

`requirements.yaml`

```yaml
roles:
  - name: notify_me
    src: https://github.com/rwxd/ansible_role_notify_me.git
    scm: git
    version: main
```

```yaml
- name: My Playbook
  hosts: all
  tasks:
    - name: Install notify-me
      ansible.builtin.include_role:
        name: notify_me
```

## Configuration

Default variables are listed under [./defaults/main.yaml](./defaults/main.yaml)
