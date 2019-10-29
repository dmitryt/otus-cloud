FROM alpine:3.10.3
RUN apk update && \
    apk add php7 php7-fpm php7-opcache && \
    mkdir -p /var/www/html && \
    addgroup -S www && \
    adduser -S www -G www

COPY php-fpm.conf /etc/php7/php-fpm.conf
WORKDIR /var/www/html

CMD ["php-fpm7", "-F"]