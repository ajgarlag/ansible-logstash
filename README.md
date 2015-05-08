ajgarlag.logstash
======================

Ansible role to install Logstash.

[![Build Status](https://travis-ci.org/ajgarlag/ansible-logstash.svg?branch=master)](https://travis-ci.org/ajgarlag/ansible-logstash)

Role Variables
--------------

* **ajgarlag_logstash_minor_version**: Minor version to configure the logstash repository (defaults to `1.4`).
* **ajgarlag_logstash_java_package**: Name of the package to install a JAVA JRE environment (defaults to `openjdk-7-jre-headless`).

Dependencies
------------

* **ajgarlag.bootstrap**: Ansible role to perform some basic setup to execute other ansible roles.

Example Playbook
----------------

```yml
- hosts: all
  roles:
    - role: ajgarlag.logstash
      ajgarlag_logstash_minor_version: 1.5
```


License
-------

MIT

Author Information
------------------

Developed with ♥ by [Antonio J. García Lagar](http://aj.garcialagar.es).
