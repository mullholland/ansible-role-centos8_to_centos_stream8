# [centos8_to_centos_stream8](#centos8_to_centos_stream8)

CentOS Linux 8 will reached End Of Life (EOL) on December 31st, 2021. This role will no longer be maintained.

Convert CentOS8 to CentOS Stream 8.
:warning: Use carefully and have a recent Backup.
Use at your own risk.


## [Role Variables](#role-variables)

These variables are set in `defaults/main.yml`:
```yaml
---
# Specialised role to convert CentOS 8 to CentOS Stream 8
# Use at your own risk
centos8_to_centos_stream8_reboot: true
centos8_to_centos_stream8_post_reboot_delay: "30"
centos8_to_centos_stream8_reboot_timeout: "300"
```


## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: Converge
  hosts: all
  become: true
  gather_facts: true
  roles:
    - role: "mullholland.centos8_to_centos_stream8"
```





## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/mullholland):

-   [centos8](https://hub.docker.com/r/mullholland/docker-molecule-centos8)

The minimum version of Ansible required is 2.10, tests have been done to:

-   The previous version.
-   The current version.
-   The development version.





If you find issues, please register them in [GitHub](https://github.com/mullholland/ansible-role-centos8_to_centos_stream8/issues)

## [License](#license)

MIT


## [Author Information](#author-information)

[Mullholland](https://github.com/mullholland)

## [Special Thanks](#special-thanks)

Template inspired by [Robert de Bock](https://github.com/robertdebock)
