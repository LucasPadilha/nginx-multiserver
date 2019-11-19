FROM php:7.1-apache

RUN apt-get update \
    && apt-get install -y --no-install-recommends git zip unzip zlib1g-dev libmcrypt-dev libpq-dev wget \
    && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install pdo_pgsql zip mcrypt

RUN a2enmod rewrite