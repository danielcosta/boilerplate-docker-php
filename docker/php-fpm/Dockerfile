FROM php:fpm-alpine

MAINTAINER Daniel Costa <danielcosta@gmail.com>

RUN echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories && \
    apk update && \
    apk upgrade && \
    apk add --update libmcrypt-dev && \
    docker-php-ext-install pdo_mysql mcrypt && \
    pecl install ds
