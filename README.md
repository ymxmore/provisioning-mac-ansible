# Provisioning mac with Ansible

## Require

Ansible >= 1.9

```bash
$ brew update
$ brew install python ansible
```

## Usage

```bash
# e.g. execute all
$ ansible-playbook playbook.yml -i hosts --become --become-user=<BECOME_USER>

# e.g. only install brew packages
$ ansible-playbook playbook.yml -i hosts --become --become-user=<BECOME_USER> --tags=brew
```
