# A container for Python3

FROM alpine:latest
MAINTAINER Amo Chumber <root.demon.net@gmail.com>

RUN apk update \
  && apk add python3 \
  && rm -rf /var/cache/apk/*

RUN python3 -m ensurepip \
  && python3 -m pip install --upgrade pip setuptools
