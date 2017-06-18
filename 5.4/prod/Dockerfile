FROM nsign/php-apache:5.4

RUN apt-get update \
    && apt-get install -y --no-install-recommends libicu52 libicu-dev \
    && docker-php-ext-install intl \
    && docker-php-ext-enable intl \

    && docker-php-ext-install pdo_mysql \
    && docker-php-ext-enable pdo_mysql \

    && apt-get autoremove -y && apt-get clean all
