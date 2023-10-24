FROM php:8.2.8-fpm-alpine3.18

COPY --from=composer /usr/bin/composer /usr/bin/composer

RUN docker-php-ext-install pdo_mysql
RUN apk add nodejs npm
RUN apk add nodejs-current
RUN cd var/www/html/backend
RUN npm install @vitejs/plugin-react react react-dom
