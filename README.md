nagios_nrpe
===========

This role deploys and configures NRPE on each host to be monitored by Nagios.
The main repo for this role is on [Le Filament GitLab](https://sources.le-filament.com/lefilament/ansible-roles/nagios_nrpe.git)

Requirements
------------

None

Role Variables
--------------

This role makes use of various variables defined in [other roles from Le Filament](https://sources.le-filament.com/lefilament/ansible-roles).
The aim being to configure all hosts defined in Ansible inventory and monitor the deployed services based on inventory groups.

Dependencies
------------

This role requires the following collection (for make module) :
* community.general

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: nagios_nrpe, tags: nrpe }

License
-------

AGPL-3

Author Information
------------------

Le Filament (https://le-filament.com)
