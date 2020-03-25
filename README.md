# Installation

```console
composer require --dev uvoteam/php-without-xdebug-runner:^1.0
```

# Usage

Assume you have installed Xdebug.

```console
$ php7.2 -v
PHP 7.2.28-3+ubuntu18.04.1+deb.sury.org+1 (cli) (built: Feb 23 2020 07:23:25) ( NTS )
Copyright (c) 1997-2018 The PHP Group
Zend Engine v3.2.0, Copyright (c) 1998-2018 Zend Technologies
    with Zend OPcache v7.2.28-3+ubuntu18.04.1+deb.sury.org+1, Copyright (c) 1999-2018, by Zend Technologies
    with Xdebug v2.9.2, Copyright (c) 2002-2020, by Derick Rethans
```

To to run php without Xdebug you can use one of provided scripts.

```console
$ vendor/bin/php7.2-no-xdebug -v
Temporary php.ini path: /tmp/php.NnsLxfuGVZ.ini
PHP 7.2.28-3+ubuntu18.04.1+deb.sury.org+1 (cli) (built: Feb 23 2020 07:23:25) ( NTS )
Copyright (c) 1997-2018 The PHP Group
Zend Engine v3.2.0, Copyright (c) 1998-2018 Zend Technologies
    with Zend OPcache v7.2.28-3+ubuntu18.04.1+deb.sury.org+1, Copyright (c) 1999-2018, by Zend Technologies
```

## PHPUnit

If you want to collect code coverage with PCOV but have installed Xdebug
then you can run PHPUnit like this:

```console
vendor/bin/php7.2-no-xdebug vendor/bin/phpunit --coverage-text
```
