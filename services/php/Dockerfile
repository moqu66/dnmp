ARG PHP_VERSION

FROM ${PHP_VERSION}

ARG PHP_EXTENSIONS

ARG TZ

ADD https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/

RUN echo 'TZ="${TZ}"; export TZ' >> /root/.profile && \
    chmod +x /usr/local/bin/install-php-extensions && \
    install-php-extensions ${PHP_EXTENSIONS}