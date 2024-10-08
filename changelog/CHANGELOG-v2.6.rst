==================================
vbotka.integrity 2.6 Release Notes
==================================

.. contents:: Topics


2.6.3
=====

Release Summary
---------------
Maintenance update.

Major Changes
-------------

Minor Changes
-------------
* Fix ansible.builtin.get_url, environment:
  CRYPTOGRAPHY_OPENSSL_NO_LEGACY: '1'
* Tasks formatting improved.



2.6.2
=====

Release Summary
---------------
Maintenance update.

Major Changes
-------------

Minor Changes
-------------
- Update python 3.11 in .travis.yml
- Update README.
- Format meta/main.yml


2.6.1
=====

Release Summary
---------------
Ansible 2.17 update

Major Changes
-------------
* Support FreeBSD 13.3, 14.0, 14.1
* Support add Ubuntu 24.04 Noble

Minor Changes
-------------
* Update README
* Use default rules in local ansible-lint config.
* Update skip_list in local ansible-lint config.
* Add variable integrity_role_version
* Update debug.yml
* Renamed tasks/packages.yml -> tasks/pkg.yml
* Renamed tasks/configure.yml -> tasks/config.yml


2.6.0
=====

Release Summary
---------------
Ansible 2.16 update.

Major Changes
-------------

Minor Changes
-------------
  
Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
