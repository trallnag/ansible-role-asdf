[![role](https://img.shields.io/ansible/role/55771)](https://galaxy.ansible.com/trallnag/asdf)
[![quality](https://img.shields.io/ansible/quality/55771)](https://galaxy.ansible.com/trallnag/asdf)
[![downloads](https://img.shields.io/ansible/role/d/55771?label=downloads)](https://galaxy.ansible.com/trallnag/asdf)

# Ansible Role `trallnag.asdf`

Ansible role that installs asdf with Git and Bash on Linux.

[asdf]: https://github.com/asdf-vm/asdf

Available on [Ansible Galaxy](https://galaxy.ansible.com/trallnag/asdf).

## Role Variables

```yaml
asdf_version:
  default: v0.8.1
  type: raw
  required: false
  description: >-
    Commit reference. Can be anything ranging from a branch name, git tag,
    or a commit id.
```

## Example Playbook

```yaml
- name: Playbook
  hosts: myhost
  remote_user: myuser
  vars:
    rolespec_validate: true
  roles:
    - name: trallnag.asdf
      vars:
        asdf_version: v0.8.1
```

## Special Requirements

* Only Bash mode supported.

## Special Dependencies

None.

## License

Apache-2.0

## Author Information

Trallnag
