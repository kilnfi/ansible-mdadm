# mrlesmithjr.mdadm

An [Ansible](https://www.ansible.com) role to install and manage [mdadm](https://linux.die.net/man/8/mdadm) raid arrays.

## ⚠️ Important: Ansible Galaxy Role Name

**As of December 2025**, this role is available on Ansible Galaxy as:

```yaml
- src: mrlesmithjr.mdadm
```

The previous duplicate role name (`mrlesmithjr.ansible-mdadm`) was removed and
consolidated into this single role. If you were using `mrlesmithjr.ansible-mdadm`,
please update your `requirements.yml` to use `mrlesmithjr.mdadm`.

**Note:** This role is used by [OpenStack Kayobe](https://docs.openstack.org/kayobe/latest/)
for software RAID management.

### Historical Download Statistics

Prior to consolidation, this role had accumulated significant usage:

| Role Name | Downloads (as of Dec 2025) |
|-----------|---------------------------|
| `mrlesmithjr.mdadm` | 632,067 |
| `mrlesmithjr.ansible-mdadm` | 8,439 |
| **Combined Total** | **640,506** |

Due to Ansible Galaxy limitations, download counts reset when roles are re-imported.
The historical data above represents the actual community usage of this role.

## Requirements

- Available unpartitioned disk devices

## Role Variables

[defaults/main.yml](defaults/main.yml)


## Dependencies

None

## Example Playbook

```yaml
- hosts: all
  become: true
  vars:
  roles:
    - role: mrlesmithjr.mdadm
  tasks:
```

## License

BSD

## Author Information

Larry Smith Jr.

- [@mrlesmithjr](https://twitter.com/mrlesmithjr)
- [mrlesmithjr@gmail.com](mailto:mrlesmithjr@gmail.com)
- [http://everythingshouldbevirtual.com](http://everythingshouldbevirtual.com)

<a href="https://www.buymeacoffee.com/mrlesmithjr" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
