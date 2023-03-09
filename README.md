# bwinfosec.add_crb
This role adds the [CodeReady Linux Builder](https://developers.redhat.com/blog/2018/11/15/introducing-codeready-linux-builder) repository to RHEL 8 hosts.

## Platforms

- RHEL 8

## Install

``` sh
ansible-galaxy collection install community.general && ansible-galaxy install bwinfosec.add_crb
```

## Example Playbook

```yml
- name: Add CodeReady Linux Builder repository to RHEL hosts
  become: true
  hosts: rhel

  roles:
    - bwinfosec.add_crb
```

## Requirements
- This role requires a valid [RHEL subscription](https://www.redhat.com/en/resources/red-hat-enterprise-linux-subscription-guide) on the target machines.
- This role depends on functionality provided by the [*community.general* ansible collection](https://github.com/ansible-collections/community.general).

## Licensing

This work is licensed under the [EUPL 1.2](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12).

## Contribution
If you want to contribute feel free to do so by creating a pull request on [github](https://github.com/bwInfoSec/ansible-role-add-crb).
