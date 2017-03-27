FROM php:7.1-fpm
#COPY ./php.ini /usr/local/etc/php
RUN docker-php-ext-install pdo_mysql


## mcrypt
#RUN runtimeRequirements="re2c libmcrypt-dev" \
#	&& apt-get update && apt-get install -y ${runtimeRequirements} \
#	&& docker-php-ext-install mcrypt \
#	&& rm -rf /var/lib/apt/lists/*
#
## mbstring
#RUN docker-php-ext-install mbstring
#
## intl
#RUN buildRequirements="libicu-dev g++" \
#	&& apt-get update && apt-get install -y ${buildRequirements} \
#	&& docker-php-ext-install intl \
#	&& apt-get purge -y ${buildRequirements} \
#	&& runtimeRequirements="libicu52" \
#	&& apt-get install -y --auto-remove ${runtimeRequirements} \
#	&& rm -rf /var/lib/apt/lists/*
#
## xdebug
#RUN yes | pecl install xdebug \
#    && echo "zend_extension=$(find /usr/local/lib/php/extensions/ -name xdebug.so)\n" > /usr/local/etc/php/conf.d/xdebug.ini \
#    && echo "xdebug.remote_enable=on\n" >> /usr/local/etc/php/conf.d/xdebug.ini \
#    && echo "xdebug.remote_autostart=off\n" >> /usr/local/etc/php/conf.d/xdebug.ini \
#    && echo "xdebug.remote_port=9000\n" >> /usr/local/etc/php/conf.d/xdebug.ini

# RUN a2enmod rewrite

#CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]