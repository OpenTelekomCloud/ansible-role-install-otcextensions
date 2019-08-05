# Ansible Role otcextensions

The role installs [python-otcextensions](https://github.com/OpenTelekomCloud/python-otcextensions) on associated server automatically. The [python-otcextensions](https://github.com/OpenTelekomCloud/python-otcextensions) enhance the native OpenStack CLI and SDK commands with further services which are provided by [Open Telekom Cloud](https://open-telekom-cloud.com/de) e.g. Auto Scaling Service (ASS), Key Management Service (KMS), Cloud Container Engine (CCE) and a lot more. With the installation of the role all necessary dependencies will be fetched, too.

## Supported OS

All supported and tested Operating Systems are listed below:

 - RedHat 7
 - CentOS 7
 - Ubuntu 18.04
 - Ubuntu 16.04
 - Fedora 30
 - Debian 9

## Sample playbook

The following example shows how to enable the role for a specific host (e.g. localhost).

    user@server:~$ cat roles/ansible-role-otcextensions/tests/test.yml
    ---
    - hosts: localhost
      roles:
        - role: ansible-role-otcextensions
          vars:
            extensions_state: present


**Important: The role is not yet published on Ansible Galaxy and needs to be downloaded locally.**
