FROM php:8.2-fpm

# installation de dépendences pour l'activation des modules nécessaires
RUN apt update \
    && apt install -y zip libzip-dev libpng-dev libicu-dev libxml2-dev

# installation des modules
RUN docker-php-ext-install mysqli pdo pdo_mysql zip intl xml

# Nettoyage du cache
RUN  apt clean