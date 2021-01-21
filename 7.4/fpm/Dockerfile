FROM php:7.4-fpm

# Install required system packages
RUN apt-get update && apt-get install -y \
    libzip-dev \
    libxml2-dev

# Install php extensions
RUN docker-php-ext-install \
    zip \
    soap \
    opcache

CMD ["php-fpm"]
