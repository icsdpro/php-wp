## [1.5.0] - 02-06-2020
### Use unix sockets instead of localhost
- Unix sockets
- Reduced image size (I forgot delete `php7.4-dev` package) 
- `keepalive 22` -> `keepalive 30`
- Increased fastcgi buffer size.

## [1.4.0] - 02-06-2020
### PHP 7.4 support
- Opcache preload support thought `$PHP_OPCACHE_PRELOAD`
- Using semver in image tag name. 
- `opcache.file_update_protection=0` as default option instead of `2`.
- `7.4-1.4.0` tag

## [1.3.0] - 02-06-2020
### PHP 7.4 support
- Drop 7.2
- Fixes some bugs
- `7.4-beta1` tag

## [1.2.0] - 30-09-2019
### Bugfixes
- Fixed opcache env variable
- Fixed logs output (Use `PHP_FPM_LOG_LEVEL` for configure it)
- Add `bcmath` and `xmlreader` extensions.
- Commented `user` and `group` options in php-fpm config

## [1.1.0] - 10-02-2019
### PHP 7.3
- Fixed failed travis build (gpg tty problem)
- Support multiple PHP versions
- Add new docker tags `php7.2-latest` and `php7.3-latest`

## [1.0.1] - 02-10-2018
### Bugfix
- Fixed container quitting when user send `Ctrl+C` input

## [1.0.0] - 21-09-2018
### First stable version
- Drop varrick template engine because his doesn't work in kubernetes cluster
- Use more fastest and stable roquie/smalte template engine
- Reduce image size
- Added NGINX_ACCESS_LOG env variable

## [0.1.0] - 15-06-2018
### First version
- Created Docker image with thrully features.
