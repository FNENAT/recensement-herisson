FROM php:8.3-fpm-alpine3.19

RUN apk update && \
    apk upgrade && \
    apk add --no-cache \ 
    libpng \
    libpng-dev \
    libzip-dev \
    && docker-php-ext-install gd \
    && docker-php-ext-install zip \
    && apk del libpng-dev
