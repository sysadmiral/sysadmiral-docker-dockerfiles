FROM alpine:latest

RUN apk update \
  && apk del python \
  && apk add python3 bash \
  && rm -rf /var/cache/apk/*

RUN python3 -m ensurepip \
  && python3 -m pip install --upgrade pip setuptools
