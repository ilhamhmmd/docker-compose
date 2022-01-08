FROM php:7.3-fpm-alpine

RUN set -ex\
    && apk --no-cache add postgresql-dev nodejs yarn\
    && docker-php-ext-install pdo pdo_pgsql

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# RUN docker-php-ext-install pdo_mysql

WORKDIR /var/www/html