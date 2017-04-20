FROM php:7-alpine

COPY index.php /app/

RUN apk add --update --no-cache libmcrypt-dev
RUN docker-php-ext-install iconv mcrypt

EXPOSE 8888

CMD ["php", "-S", "0.0.0.0:8888", "/app/index.php"]] 

