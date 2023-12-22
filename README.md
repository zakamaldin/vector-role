vector-role
=========

This role can install vector service on machine

Role Variables
--------------

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `vector_version` | 0.34.0 | Version of Vector service, which will be download and install on machine |

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: vector-role}

License
-------

MIT

Author Information
------------------

Zakamaldin Andrey
