phpfpm
======

PHP-FPM (FastCGI Process Manager) is an alternative PHP FastCGI implementation
with some additional features useful for sites of any size, especially busier
sites.

Samples
-------
```
include phpfpm
```
```
phpfpm::config {
  'global/error_log': value => '/var/log/php-fpm/error.log';
  'global/daemonize': value => 'yes';
}
```
```
phpfpm::modules { 'php-pear-PHP-CodeSniffer': ensure => 'latest' }
phpfpm::modules { 'php-gd': ensure => 'latest' }
phpfpm::modules { 'php-ldap': ensure => 'latest' }
phpfpm::modules { 'php-mbstring': ensure => 'latest' }
phpfpm::modules { 'php-mcrypt': ensure => 'latest' }
phpfpm::modules { 'php-mysql': ensure => 'latest' }
phpfpm::modules { 'php-xml': ensure => 'latest' }
```

License
-------
GPL3

Contact
-------
breauxaj AT gmail DOT com