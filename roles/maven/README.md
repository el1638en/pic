maven
=========

Maven install role.

Requirements
------------

None.

Role Variables
--------------

| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|maven_version|3.5.0|Maven version|
|maven_archive_name|maven-3.5.0-bin.tar.gz|Archive .tar.gz |
|maven_download_archive_url|-| URL to download maven|
|maven_install_directory|/opt/maven|Maven install directory|
|maven_home|/opt/maven/apache-maven-3.3.9|Maven absolut path|
|maven_home|maven_settings_servers|Credentials which will be add to settings.xml|

Dependencies
------------

None.

Example Playbook
----------------

Install maven

    - hosts: servers
      roles:
         - { role: maven }

License
-------

BSD

Author Information
------------------

Eric LEGBA.