Apache Brotli
=========

Install Apache Brotli module.

Requirements
------------

You should have Apache2 installed.

Role Variables
--------------

Optionnals : 

* apache_brotli_log_format

Example : `apache_brotli_log_format: "\"%r\" %{brotli_out}n/%{brotli_in}n (%{brotli_ratio}n)"` will outpout `LogFormat '"%r" %{brotli_out}n/%{brotli_in}n (%{brotli_ratio}n)' brotli`.

* apache_brotli_custom_log

Example : `apache_brotli_custom_log: "${APACHE_LOG_DIR}/brotli_access.log"` will outpout `CustomLog ${APACHE_LOG_DIR}/brotli_access.log brotli`.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - { role: jygastaud.apache-ondrej }
        - { role: jygastaud.apache-brotli }

License
-------

MIT

Author Information
------------------

This role was created in 2017 by [Jean-Yves Gastaud](http://gastaud.io).
