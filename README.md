Deploy user
========

Creates deployment user with key authentication.

Installation
--------------

`ansible-galaxy install palkan.deploy_user`

Role Variables
--------------

| Name              | Default | Description    |
|-------------------|---------|----------------|
| deploy_user       | deployer| User name      |
| deploy_user_sudo  | true    | Whether to add user to sudoers |
| deploy_user_key   |  | Path to key file (**required**) |

Example Playbook
-------------------------
```yml
  - hosts: servers
    roles:
       - palkan.deploy_user
```
