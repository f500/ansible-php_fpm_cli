php\_fpm\_cli
=============

Install `libfcgi` (which provides `cgi-fcgi`) and [`php-fpm-cli`][3].

`php-fpm-cli` is a tool to have PHP FPM run arbitrary code from the command line.
We use this tool in our `f500.php_opcache_reset` role to reset the OPcache which lives in FPM's memory.

Not much else to tell here, but please take a look at the role [`f500.php_opcache_reset`][1].

Many thanx to [Mathias Leppich][2], who is the author of [`php-fpm-cli`][3] and gave us the idea to create these roles!


Requirements
------------

None, but this role is only usefull when you use the PHP FPM.


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

#### This role

[LGPLv3][5]

#### [Mathias Leppich][2]'s [php-fpm-cli][3] tool

[MIT][3]


Author Information
------------------

#### This role

Jasper N. Brouwer, jasper@future500.nl

Ramon de la Fuente, ramon@future500.nl


#### [Mathias Leppich][2]'s [php-fpm-cli][3] tool

Mathias Leppich, mleppich@muhqu.de

[1]: https://galaxy.ansible.com/list#/roles/1146
[2]: https://github.com/muhqu
[3]: https://gist.github.com/muhqu/91497df3a110f594b992
[4]: http://php.net/manual/en/book.fpm.php
[5]: https://github.com/f500/ansible-php_fpm_cli/blob/master/COPYING.LESSER
