Role Name
========

The purpose of this role is to install kune to a web server and enable access
with nginx. The kune server name can be specified by changing the kune_hostname
variable in vars/main.yml.

Role Variables
--------------

- kune_hostname: hostname that kune will service, will be set to "kune" by
                 default
- kune_port: portname that kune will service, will be set to 8888 by default.
- kune_root_mysql_password: root mysql password, will be set to a random value 
                            by default.
- kune_kune_mysql_password: kune mysql password, will be set to a random value 
                            by default

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables 
passed in as parameters) is always nice for users too:

    - hosts: default
      sudo: True
      roles:
        - kune

Try it Out
---------------------------

Check out the github repository, vagrant up, and load http://localhost:8888 in
your web browser.

License
-------

Affero GPL

Author Information
------------------

http://marklee77.github.io

