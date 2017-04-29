Debian-PhpNewRelicExtension
===========================

Application Performance Management & Monitoring

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

newrelic:
  license: "xxxxxxxxxxxxx"
  appname: "Application Name"

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-php-newrelic, newrelic.license: "xxxxxxxxxxxxx", newrelic.appname: "Application Name" }

Tasks
-----

  - Register NewRelic [APT repository](https://docs.newrelic.com/docs/php/php-agent-installation-ubuntu-and-debian)
  - Install [newrelic](https://docs.newrelic.com/docs/php/new-relic-for-php) php extension
  - Apply newrelic configuration

License
-------

BSD
