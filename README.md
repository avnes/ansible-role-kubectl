# ansible-role-kubectl

Ansible role for installing kubectl.

## Requirements

Poetry. Install it from <https://python-poetry.org/docs/>

## Role Variables

```yaml
kubectl_version: latest     # It can also be a specifik version like v1.21.4
kubectl_for_all_users: true # If false it will install in in the users ~/bin directory
```

## Dependencies

None

## Example Playbook

```yaml
- hosts: all
  roles:
     - { role: avnes.kubectl }
```

## Test

```bash
poetry install
poetry shell
molecule test
```

## License

MIT

## Author Information

<https://github.com/avnes>
