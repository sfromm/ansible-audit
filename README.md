Audit
=====

Ansible role to manage linux [audit](http://people.redhat.com/sgrubb/audit/) daemon.

Requirements
------------

None.

Role Variables
--------------

- **audit_rules** - Apply the given audit rules to a host.  Current
  options are: *capp*, *lspp*, *nispom*, and *stig*.  The default is
  *null*, which is basically an empty ruleset.

Dependencies
------------

None.

Example Playbook
----------------

A simple example

    - hosts: servers
      roles:
         - { role: sfromm.audit, audit_rules: stig }

License
-------

GPLv2

Author Information
------------------

See https://github.com/sfromm
