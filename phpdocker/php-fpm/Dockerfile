FROM phpdockerio/php71-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php-memcached php7.1-mysql php7.1-sqlite3 php7.1-bcmath php7.1-bz2 php7.1-gd php7.1-gmp php-imagick php7.1-mbstring php7.1-odbc php7.1-phpdbg php-ssh2 php7.1-xmlrpc php-yaml \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


WORKDIR "/var/www/ttblog"