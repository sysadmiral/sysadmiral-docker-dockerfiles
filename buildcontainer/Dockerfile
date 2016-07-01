# A container based on Alpine Linux that includes bundler (rubygems), \
# npm (nodejs) and composer (php)

FROM alpine:latest
MAINTAINER Amo Chumber <root.demon.net@gmail.com>

RUN apk add --no-cache \
  ruby-bundler \
  nodejs-lts \
  curl \
  php5 \
  php5-openssl \
  php5-json \ 
  php5-phar \
  python3 \
  && curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer

CMD /bin/sh
