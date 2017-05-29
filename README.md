Ansible Role: Certbot
=========

[![Build Status](https://travis-ci.org/CarlosLongarela/ansible-role-certbot.svg?branch=master)](https://travis-ci.org/CarlosLongarela/ansible-role-certbot)
[![Percentage of issues still open](http://isitmaintained.com/badge/open/CarlosLongarela/ansible-role-certbot.svg)](http://isitmaintained.com/project/CarlosLongarela/ansible-role-certbot "Percentage of issues still open")
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/CarlosLongarela/ansible-role-certbot.svg)](http://isitmaintained.com/project/CarlosLongarela/ansible-role-certbot "Average time to resolve an issue")

Certbot installation and dhparam.pem generation.

Requirements
------------

None.

Role Variables
--------------

    aptget_update_cache_valid_time: 3600

    certbot_cron:
      minute: "3"
      hour: "4"
      day: "*"
      weekday: "0"

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers

      gather_facts: no
      become: true

      roles:
         - { role: CarlosLongarela.certbot}

License
-------

GPLv2

Author Information
------------------

This role was created in 2017, May by [Carlos Longarela](mailto:carlos@longarela.eu), from [Taberna WordPress](https://tabernawp.com/).
