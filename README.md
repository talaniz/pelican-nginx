Pelican Nginx Role
==================

A role to setup Nginx to server Pelican static files.

Requirements
------------

Ansible version 16+ as the ufw module is used.

Variables
---------

* `nginx`: location of the nginx installation (/etc/nginx/nginx.conf)
* `files_dir`: location of files to transfer nginx.conf
* `templates_dir`: location of templates to transfer default file

Example Playbook
----------------

    - hosts: servers
      vars:
         - files_dir: ~/ansible/playbooks/files
         - templates_dir: ~/ansible/playbooks/templates
      roles:
         - talaniz.pelican-nginx

License
-------

BSD

Author Information
------------------
E-mail: antonio.alaniz@gmail.com
Website: www.antonioalaniz.com

