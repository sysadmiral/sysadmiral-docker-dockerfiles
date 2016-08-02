# A container for the excellent donnemartin/saws
#
# See: https://github.com/donnemartin/saws

FROM alpine:latest
MAINTAINER Amo Chumber <root.demon.net@gmail.com>

ENV latest_saws_version="0.4.0"

RUN apk add --no-cache \
  git \
  python3

RUN python3 -m pip install --upgrade --no-cache-dir pip
RUN python3 -m pip install --no-cache-dir git+https://github.com/donnemartin/saws.git@$latest_saws_version

ENTRYPOINT ["saws"]
