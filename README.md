# superset

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-superset.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for superset

This role was prepared and tested for Ubuntu 18.04.

# Installation

`$ ansible-galaxy install insight_infra.superset`

# Default settings

```
superset_version: 0.37.0
superset_username: user
superset_password: password
superset_firstname: John
superset_lastname: Doe
superset_email: email@example.com

superset_app: superset
superset_flask_secret_key: changeme
superset_port: 8088
superset_workers: 2
superset_mapbox_api_key: changeme
superset_secret_key: changeme

superset_auth_type: AUTH_DB
superset_oauth_providers:
superset_service_env_vars:
superset_service: /etc/systemd/system/superset.service

superset_user: superset
superset_group: superset

superset_user_shell: /bin/bash # Change to '/bin/false' in production

python_version: 3.6
superset_path: /opt/superset
superset_venv_path: /opt/superset/env
superset_python_path: "{{ superset_venv_path }}/bin/python  {{ superset_venv_path }}/bin/superset"

superset_postgres_db_host: localhost
superset_postgres_db_port: 5432
superset_postgres_db_username: superset
superset_database: postgres
superset_postgres_db_password: changeme

superset_load_examples: false

superset_languages:
  - key: en
    flag: us
    name: English
```