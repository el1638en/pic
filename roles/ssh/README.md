ssh
=========

Install & configure ssh.

Requirements
------------

None.

Role Variables
--------------

| Nom	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|ssh_delete_obsolete_packages|False|Yes/No delete obsolete package.|
|ssh_package|openssh-server|Ssh package.|
|ssh_banner_information|Linux SSH Server|SSH Banner information.|
|ssh_tmout|900|After 900 seconds of inactivity, the ssh connexion is disabled|
|ssh_histsize|20|.|
|ssh_histfilesize|20|.|
|ssh_motd_file|/etc/motd|The Message Of The Day.|
|ssh_banner_file|/etc/ssh/ssh_banner|SSH Banner.|
|ssh_profile_file|/etc/profile|Profile file address.|
|ssh_config_port|22|SSH TCP port.|
|ssh_config_file|/etc/ssh/sshd_config|SSH Config file.|
|ssh_goss_enabled|False|Enable/Disable Goss test after installation.|
|ssh_version|6.7|SSH version.|
|ssh_version_support_etm|6.3|SSH version support ETM.|
|ssh_macs_etm|MACs hmac-sha2-512-etm@openssh.com,hmac-sha2-256-etm@openssh.com,hmac-sha1|MAC ETM algorithm.|
|ssh_macs_old|MACs hmac-sha1|Old MAC Algorithm.|
|ssh_config|list|List of configuration directives for SSH.|
|ssh_issue_files|list|List of issue files.|


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ssh }

License
-------

BSD

Author Information
------------------

Eric LEGBA.