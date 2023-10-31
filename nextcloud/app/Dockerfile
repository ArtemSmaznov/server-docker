FROM nextcloud:fpm-alpine

RUN apk add --no-cache procps samba-client
RUN echo '0 4 * * * php /var/www/html/occ preview:pre-generate' >> /var/spool/cron/crontabs/www-data
