FROM php:8.1.22-apache

COPY 000-default.conf /etc/apache2/sites-enabled/

RUN apt-get update && apt-get install -y libpq-dev git && docker-php-ext-install pdo pdo_pgsql

RUN pecl install xdebug && docker-php-ext-enable xdebug

COPY xdebug.ini /usr/local/etc/php/conf.d/xdebug.ini

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer