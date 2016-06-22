ansible-role-timezone
=====================

Set timezone and optionally enable NTP on a host.
Uses timedatectl to perform task; on RedHat and CentOS still uses regular ntp(d) since their systemd is compiled with systemd-timesyncd explicitely turned off.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

    timezone: "Europe/Berlin"

Set timezone to String.

    enable_ntp: true

Whether to enable NTP.


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      vars_files:
        - vars/main.yml
      roles:
         - { role: azmodude.timezone }

License
-------

BSD

Author Information
------------------

None.
