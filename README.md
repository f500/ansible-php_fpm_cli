php\_fpm\_cli
=============

Install `libfcgi` (which provides `cgi-fcgi`) and `php-fpm-cli`, which are needed for the role `f500.php_opcache_reset`.

Not much to tell here, but please take a look at the role `f500.php_opcache_reset`.

Many thanx to [Mathias Leppich][2], who is the author of [php-fpm-cli][3] and gave us the idea to create the role `f500.php_opcache_reset`!


Requirements
------------

None.


Role Variables
--------------

None.


Dependencies
------------

None.


Example Playbook
----------------

Use as is:

    - hosts: servers
      roles:
         - { role: f500.php_fpm_cli }

License
-------

### This role

LGPLv3

### [Mathias Leppich][2]'s [php-fpm-cli][3] script

MIT


Author Information
------------------

### This role

Jasper N. Brouwer, jasper@nerdsweide.nl

### [Mathias Leppich][2]'s [php-fpm-cli][3] script

Mathias Leppich, mleppich@muhqu.de

[1]: https://galaxy.ansible.com/list#/roles/xxx
[2]: https://github.com/muhqu
[3]: https://gist.github.com/muhqu/91497df3a110f594b992
