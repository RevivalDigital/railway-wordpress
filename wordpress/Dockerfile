FROM wordpress:php8.3-apache

# Konfigurasi PHP (upload size, memory, dll)
COPY php-custom.ini /usr/local/etc/php/conf.d/zz-custom.ini

# Hilangkan warning ServerName Apache
RUN echo "ServerName localhost" > /etc/apache2/conf-available/servername.conf \
 && a2enconf servername
