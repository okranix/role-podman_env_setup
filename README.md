Podman environment setup
=========

Configure podman user to allow rootless containers and privlieged port usage.

Requirements
------------

None

Role Variables
--------------

| Name                         | Comment                                                   | Default value  |
|------------------------------|-----------------------------------------------------------|----------------|
| podman_user        | Username of the user running the containers                         | `ansible`      |

Dependencies
------------

- ansible-galaxy collection install ansible.posix

Example Playbook
----------------

    ---
    - name: Podman setup
      hosts: podman_hosts
      roles:
        - role: role-podman_env_setup

License
-------

BSD
