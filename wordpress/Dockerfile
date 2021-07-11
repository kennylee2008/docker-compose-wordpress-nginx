FROM wordpress:php7.4-fpm
RUN usermod -u 1005 www-data && groupmod -g 1005 www-data
RUN chown -R 1005:1005 /var/www/html