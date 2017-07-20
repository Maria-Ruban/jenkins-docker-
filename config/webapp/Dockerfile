# Use php:7.0-apache2 as base image to build custom Infanion image
FROM php:7.0-apache

RUN apt-get update && apt-get install -y libpng-dev && docker-php-ext-install gd mbstring opcache pdo pdo_mysql && a2enmod rewrite

COPY opcache.ini /usr/local/etc/php/opcache.ini

WORKDIR /var/www/html
