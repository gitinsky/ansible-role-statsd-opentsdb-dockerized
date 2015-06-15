FROM gitinsky/baseimage:0.1.5
MAINTAINER Git In Sky <support@gitinsky.com>

RUN \
  apt-get update && apt-get -y install nodejs npm && \
  npm install statsd-opentsdb-backend && \
  cd / && \
  git clone https://github.com/etsy/statsd.git && mkdir /statsd/config

COPY start.sh /start.sh

CMD ["/start.sh"]
