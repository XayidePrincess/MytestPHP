FROM php:fpm

RUN apt-get update
RUN docker-php-ext-install pdo pdo_mysql
RUN apt-get install -y zlib1g-dev libicu-dev g++ \
    && docker-php-ext-configure intl \
    && docker-php-ext-install intl