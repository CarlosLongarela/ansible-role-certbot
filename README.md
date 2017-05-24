Ansible Role: Certbot
=========

[![Build Status](https://travis-ci.org/CarlosLongarela/ansible-role-certbot.svg?branch=master)](https://travis-ci.org/CarlosLongarela/ansible-role-certbot)

Certbot installation and dhparam.pem generation.

Requirements
------------

None.

Role Variables
--------------

    aptget_update_cache_valid_time: 3600

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
