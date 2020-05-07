FROM devilbox/php-fpm-8.0:latest

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www/default/htdocs
