FROM nextcloud:fpm-alpine

RUN echo '*/5 * * * * php -f /var/www/nextcloud/cron.php' > /var/spool/cron/crontabs/www-data 
