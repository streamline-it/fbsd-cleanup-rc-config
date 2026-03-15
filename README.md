Role Name
=========

Organizes the /etc/rc.conf file.  Uses a template to populate an origanized rc.conf while also giving the option to back the file up.

Requirements
------------

Compatible with RHEL7 - 9.  And with FreeBSD 13 - 15

Role Variables
--------------

# defaults file for fbsd-cleanup-rc-config

# path to rc config
fbsd_cleanup_rc_config_rc_dest: /etc/rc.conf
fbsd_cleanup_rc_config_rc_src: /etc/rc.conf

# if true the rc.conf file will be backed up
fbsd_cleanup_rc_config_backup_conf: true

# used to define sections of the rc.conf
fbsd_cleanup_rc_config_section_1: []
fbsd_cleanup_rc_config_section_2: []
fbsd_cleanup_rc_config_section_3: []
fbsd_cleanup_rc_config_section_4: []
fbsd_cleanup_rc_config_section_5: []

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: servers
  
  vars:

    fbsd_cleanup_rc_config_backup_conf: false 

  roles:
    - fbsd_cleanup_rc_config

License
-------

BSD

Author Information
------------------

Rich O'Hara
