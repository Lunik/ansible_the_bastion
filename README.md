OVH The Bastion
=========

Deploy OVH The Bastion on a server.

Requirements
------------

A server with Ubuntu 22.04

Install the role with :

```bash
ansible-galaxy install lunik.the_bastion
```

Role Variables
--------------

See `defaults/main.yml` for the list of variables.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- name: "Test"
  hosts: bastion
  gather_facts: true
  become: true
  vars:
    bastion_admin: wabbit
    bastion_admin_ssh_pubkey: 'ssh-rsa XXXXXXXXXX'
  roles:
    - name: lunik.the_bastion
```

License
-------

GPLv3

Author Information
------------------

Guillaume MARTINEZ <lunik@tiwabbit.fr>
