## install laravel

## install php php-pear & php-dev

## install laravel octane

## install swoole via pecl
php --ri openswoole
$ pecl install -D 'enable-sockets="no" enable-openssl="yes" enable-http2="yes" enable-mysqlnd="yes" enable-swoole-json="no" enable-swoole-curl="yes" enable-cares="yes" with-postgres="yes"' openswoole

## install libcurl4-openssl-dev


# Check the loaded CLI php.ini config file location
$ php -i | grep php.ini (linux)

## enable swoole extention in PHP 
extension=/usr/lib/php/20210902/swoole.so
extension=/usr/lib/php/20210902/openswoole.so


## install php-swoole


## install road runner
composer require spiral/roadrunner

## install octane
php artisan octane:install

## start octane
php artisan octane:start --server=roadrunner --host=127.0.0.1 --port=8002 
php artisan octane:start --server=swoole --host=127.0.0.1 --port=8001


## test benchmark using wrk
wrk -t4 -c50 -d10s http://127.0.0.1:8001/api/blog

