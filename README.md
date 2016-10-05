Java
====

Installs Oracle Java

Requirements
------------

No external requirements.

Role Variables
--------------

* `java_version`: Desired major version (8)
* `java_install_dir`: Location  to install to (/opt)
* `java_download_dir`: Location to download tarball to (/tmp)
* `java_set_default`: Set "/opt/java" symlink (true)
* `java_set_compatibility_symlink`: _(optional)_ Set "/usr/local/bin" symlink
* `java_webproxy`: _(optional)_ HTTP/HTTPS Proxy information

Dependencies
------------

No external roles required.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ucsdlib.java, java_install_dir: /usr/local }

License
-------

BSD 2 Clause

Author Information
------------------

John H. Robinson, IV  
The Library  
UC San Diego  
