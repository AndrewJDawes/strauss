FROM php:8.4-cli

RUN apt-get update && apt-get install -y --no-install-recommends \
    wget \
    git \
    unzip \
    curl \
    && rm -rf /var/lib/apt/lists/*

COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer
