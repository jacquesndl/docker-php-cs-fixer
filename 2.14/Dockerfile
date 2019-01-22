FROM php:7.1-alpine

ENV PHP_CS_FIXER_VERSION=2.14.0

RUN curl -L https://github.com/FriendsOfPHP/PHP-CS-Fixer/releases/download/v$PHP_CS_FIXER_VERSION/php-cs-fixer.phar > /usr/local/bin/php-cs-fixer \
    && chmod +x /usr/local/bin/php-cs-fixer
RUN rm -rf /var/cache/apk/* /var/tmp/* /tmp/*

WORKDIR /app
ENTRYPOINT ["php-cs-fixer"]
