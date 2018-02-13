postgres
=========

postgres role installs postgresql server.

Requirements
------------
None.

Role Variables
--------------

| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|postgres_version|9.6|PostgreSQL server version.|
|postgres_listen_addresses|*|Listen IP address.|
|postgres_server_pkg|postgresql-9.6|PostgreSQL server package.|
|postgres_client_pkg|postgresql-client-9.6|PSQL client package.|
|postgres_port|5432|PostgreSQL server port.|
|postgres_conf_dir|/etc/postgresql/{{ postgres_version }}/main|PostgreSQL configuration directory.|
|postgres_pg_hba_file|{{postgres_conf_dir}}/pg_hba.conf|PostgreSQL pg_hba.conf file.|

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: postgres }

License
-------

BSD

Author Information
------------------

Eric LEGBA.