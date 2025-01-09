FROM php:8.2-apache

WORKDIR /var/www/html

# Enable rewrite mode
RUN a2enmod rewrite

RUN apt update \
&& apt install -y apt-utils vim curl wget \
&& pecl install xdebug 

ADD ./php/php.ini /usr/local/etc/php/

# MySQL
RUN docker-php-ext-install pdo pdo_mysql mysqli

RUN docker-php-ext-enable xdebug

ENV XDEBUG_MODE=debug

EXPOSE 80