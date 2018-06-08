Role Name
=========

Un role qui monte un docker-compose avec trois containers:
-apache
-mariadb
phpmyadmin

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
Les variables du roles se définissent dans ver/main.yml
les variables par défaut sont:
repertoire_projet: ou se trouve le projet par defaut /opt
data_base: nom de la base de donnée par defaut wordpress
user: nom utilisatuer par défaut wordpress
password: mdp par défaut secret

les ports de redirection des services des containers par défaut:
80 pour apache
8080 pour phpmyadmin
3306 pour mariadb


Installation de Wordpress
-------------------------
l'hote de la base de donnée est db

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
