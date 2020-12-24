FROM php:7.4

# Install required system packages
RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libxml2-dev

# Install php extensions
RUN docker-php-ext-install \
    zip \
    soap \
    opcache

# Install composer
COPY --from=composer /usr/bin/composer /usr/bin/composer
