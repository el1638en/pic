sonarqube
=========

sonarqube.

Requirements
------------

None.

Role Variables
--------------


| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|sonarqube_version|6.7|SonarQube version.|
|sonarqube_install_directory|/opt/sonar|SonarQube installation directory.|
|sonarqube_archive_name|sonarqube-{{sonarqube_version}}.zip|SonarQube archive name.|
|sonarqube_download_archive_url|-| URL where download SonarQube archive.|
|sonarqube_home|/opt/sonar/sonarqube-{{sonarqube_version}}|SonarQube home directory.|
|sonarqube_postgres_database_enabled|False|Enable/Disable SonarQube to store its datas into postgres database.|
|sonarqube_postgres_host|localst|postgres database address.|
|sonarqube_postgres_username|sonar|Postgres database username.|
|sonarqube_postgres_password|sonar|Pstgres database password.|
|sonarqube_postgres_database|sonar|Postgres database where sonar will store his datas.|
|sonarqube_postgres_jdbc_url|jdbc:postgresql://{{sonarqube_postgres_host}}/{{ sonarqube_postgres_database }}|Postgres database URL.|
|sonarqube_postgres_config|-|Postgres database config.|
|sonarqube_web_port|9000|SonarQube web port.|
|sonarqube_iptables_enabled|False|If `True`, open `sonarqube_web_port` by iptables.|
|sonarqube_network_interface|eth0|Netwaork interface where iptables rule will be apply.|


Dependencies
------------

none.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

Eric LEGBA.
