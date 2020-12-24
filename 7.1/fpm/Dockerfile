FROM php:7.1-fpm

# Install required system packages
RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libxml2-dev

# Install php extensions
RUN docker-php-ext-install \
    zip \
    soap \
    opcache
