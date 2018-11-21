Webapp
======

Deploy web application with buildpacks.

This roles deploys web applications in a PaaS-like environment using:
- Heroku buildpacks.
- Capistrano-like directories.
- Configuration options as environment variables.
- Systemd for process management.

Multiple buildpacks are supported to allow for applications that use multiple languages or need utilities written a different language from the main application.

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
- Generalize use of env variables using `env.d` and ansible's `assemble` module.
- Support systemd alternatives, ie monit, supervisor, pm2, etc...
- Fix idempotency with capistrano-like directories.
- Document defaults.

Licence
-------
Released under the [MIT license](https://opensource.org/licenses/MIT).

Author Information
------------------
Luis Gracia while at [EMBL-EBI](http://www.ebi.ac.uk/):
- luis.gracia [at] ebi.ac.uk
- GitHub at [luisico](https://github.com/luisico)
- Galaxy at [luisico](https://galaxy.ansible.com/luisico)
