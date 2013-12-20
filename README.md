ansible-postgres
================

Ansible Galaxy role for PostgreSQL.

This role does the installation from the PostgreSQL apt repository. Once installed, there is no config done. It is supposed to be done via **ansible-pull** from a private repository.

The use of this role is mainly to provide an easy way to build a Docker container with PostgreSQL installed. The configuration its made upon deploy.

# Requirements

Ansible 1.4.2 or higher.

# Examples

1. Default installation

    - hosts: database
      roles: jllopis.postgres

2. Specifying PostgreSQL version

   - hosts: database
     roles: jllopis.postgres
     pgversion: "9.3"


