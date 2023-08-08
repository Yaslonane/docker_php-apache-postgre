FROM php:8.1.22-apache
RUN apt-get update && apt-get install -y libpq-dev && docker-php-ext-install pdo pdo_pgsql




#FROM php:fpm-alpine
#RUN apk update; \
#    apk upgrade;
#RUN apk add --n0-cache curl git build-base zlib-dev oniguruma-dev autoconf bash

#COPY --from=composer:latest /usr/bin/composer /usr/bin/composer



#RUN docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
#    && docker-php-ext-install pgsql pdo_pgsql