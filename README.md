# curl

Ansible role to install `curl` on Ubuntu systems.

## Requirements

None. Uses only `ansible.builtin` modules.

## Role Variables

| Variable | Default | Description |
|---|---|---|
| `curl_package` | `curl` | Package name to install |
| `curl_state` | `present` | `present` to install, `absent` to remove |

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  become: true
  roles:
    - role: jeffrey.curl
```

## Overriding Variables

```yaml
- hosts: all
  become: true
  roles:
    - role: jeffrey.curl
      vars:
        curl_state: absent   # uninstall curl
```

## License

MIT

## Author

jeffrey
