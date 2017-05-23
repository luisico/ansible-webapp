Webapp
======

Deploy web application with buildpacks.

This roles deploys web applications in a PaaS-like environment using:
- Heroku buildpacks.
- Capistrano-like directories.
- Configuration options as environment variables.
- Systemd for process management.

Requirements
------------
See `meta/main.yml`.

Role Variables
--------------
See `defaults/main.yml`.

Dependencies
------------
None.

Example Playbook
----------------
Example:
```
- hosts: servers
  roles:
    - webapp
```

TODO
----
- Generalize use of buildpacks.
- Generalize use of env variables using `env.d` and ansible's `assemble` module.
- Support systemd alternatives, ie monit, supervisor, pm2, etc...
- Fix idempotency with capistrano-like directories.

Licence
-------
Licensed under [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

Author Information
------------------
Luis Gracia while at [EMBL-EBI](http://www.ebi.ac.uk/):
- luis.gracia [at] ebi.ac.uk
- GitHub at [luisico](https://github.com/luisico)
- Galaxy at [luisico](https://galaxy.ansible.com/luisico)
