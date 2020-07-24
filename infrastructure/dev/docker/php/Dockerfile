FROM phpearth/php:7.3-nginx

COPY php.ini /etc/php/7.3/conf.d/walleteye.ini
COPY www.conf /etc/php/7.3/php-fpm.d/www.conf
COPY nginx/default.conf /etc/nginx/conf.d/default.conf

RUN apk update
RUN apk add --no-cache composer php7.3-redis php7.3-pdo php7.3-pdo_pgsql php7.3-xdebug
