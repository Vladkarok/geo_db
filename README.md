Geo citizen database
=========

This role installing PostgreSQL server (default version 12), creates user, database and passwords on Centos 7

Requirements
------------

Tested in AWS EC2, other environment does not guarantee proper working, but you can test.  
Role Variables
--------------

> This role requires following variables:  
```
db_user: DATABASE_USERNAME
db_password: DATABASE_USER_PASSWORD
db_name: DATABASE_NAME
```
You can insert them in your playbook as you want
Dependencies
------------

Geo citizen web server ansible role should be used to configure full project
Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- name: DB
  hosts: db
  become: true
  vars_files: secret_vars.yml
  roles:
    - geo_db
```    
    

License
-------

MIT

Author Information
------------------
Vladyslav Karpenko
