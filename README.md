Java Oracle
=========

Simple role to install Oracle Java from url. RPM is downloaded to /tmp and installed with yum.

Role Variables
--------------

defaults/main.yml:
java_oracle_url: http://download.oracle.com/otn-pub/java/jdk/8u121-b13/e9e7ea248e2c4826b92b3f075a80e441/jre-8u121-linux-x64.rpm
java_oracle_rpm: {{ java_oracle_url | basename }}


Example Playbook
----------------

As depedency for other projects or:

    - hosts: servers
      roles:
         - { role: NLCR.java-oracle, java_oracle_url: http://download.oracle.com/otn-pub/java/jdk/8u121-b13/e9e7ea248e2c4826b92b3f075a80e441/jre-8u121-linux-x64.rpm }

License
-------

BSD

Author Information
------------------

Rudolf Kreibich, https://github.com/westfood/
