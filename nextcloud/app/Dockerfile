FROM nextcloud:fpm-alpine

VOLUME /var/www/nextcloud

WORKDIR /var/www/nextcloud

CMD sed -i 's/\/var\/www\/html/\/var\/www\/nextcloud/' /entrypoint.sh && \
    echo '*/5 * * * * php -f /var/www/nextcloud/cron.php' > /var/spool/cron/crontabs/www-data && \
    /entrypoint.sh php-fpm
