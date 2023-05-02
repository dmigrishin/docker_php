FROM php:7.4-fpm
LABEL maintainer="Dmitrii Grishin"
RUN apt-get update && \
    apt-get install -y \
        curl \
        wget \
        git

WORKDIR /srv/code/

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN chown -R www-data:www-data /srv/code