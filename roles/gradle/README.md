gradle
=========

Installation of Gradle.

Requirements
------------

None.

Role Variables
--------------

| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|gradle_version|3.5|Gradle Version|
|gradle_archive_name|gradle-3.5-all.zip|Archive .zip name|
|gradle_download_archive_url|https://services.gradle.org/distributions/gradle-3.5-all.zip|Url of the archive|
|gradle_install_directory|/opt/gradle|Installation directory|
|gradle_home|/opt/gradle/gradle-3.5|Absolut path of the archive name|

Dependencies
------------

None.

Example Playbook
----------------

Install gradle

    - hosts: all
      roles:
        - { role: gradle }

License
-------

BSD

Author Information
------------------

Eric LEGBA.
