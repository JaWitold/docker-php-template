FROM php:8.1.7-fpm

# RUN apt-get update && apt-get install -y software-properties-common
# RUN add-apt-repository ppa:ondrej/php

RUN apt-get update && apt-get install -y git zip unzip
RUN docker-php-ext-install pdo_mysql && docker-php-ext-enable pdo_mysql
# xdebug
RUN pecl install xdebug && docker-php-ext-enable xdebug

WORKDIR /var/www