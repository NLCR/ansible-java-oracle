Oracle Java
=========

Simple role to install Oracle Java from url.

Role Variables
--------------

defaults/main.yml:
oracle_java_url: http://download.oracle.com/otn-pub/java/jdk/8u121-b13/e9e7ea248e2c4826b92b3f075a80e441/jre-8u121-linux-x64.rpm
oracle_java_rpm: {{ oracle_java_url | basename }}


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

Rudolf Kreibich, https://github.com/westfood/
