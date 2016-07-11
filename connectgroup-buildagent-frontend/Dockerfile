FROM centos:7
MAINTAINER WebOps <webops@connect-group.com>

RUN set -ex \
  && curl --silent --location https://rpm.nodesource.com/setup_4.x | bash - \
  && yum install -y nodejs gcc-c++ make rubygem-bundler git \
  && gem install rubygems-update \
  && update_rubygems \
  && gem update --system \
  && gem install bundler \
  && npm install --global gulp-cli \
  && yum clean all

ENTRYPOINT ["/bin/sh"]
