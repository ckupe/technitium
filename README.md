ckupe.technitium
=========

Configures containerized technitium-dns on linux distros with firewalld and systemd-resolved.

Requirements
------------

- Podman 4.x+ (To support Quadlet)
- systemd-resolved
- firewalld

Role Variables
--------------


| variable | description | default |
|--|--|--|
| technitium_config_dir | config directory you want to write the deployment.yaml file to, which systemd will invoke with podman to deploy the stack. | /opt/technitium |
| technitium_service_name | desired systemd service name | technitium



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: ckupe.technitum
           vars:
             technitium_config_dir: /opt/mydir
             technitium_service_name: my-technitium

License
-------

GPL-v3

Author Information
------------------

Chris Kuperstein (chris@kuperstein.net)
