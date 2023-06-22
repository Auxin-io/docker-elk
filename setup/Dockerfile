ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:8.2.0

USER root

COPY . /

RUN set -eux
RUN	mkdir /state
COPY setup /state
RUN	chown elasticsearch /state
WORKDIR /setup

USER elasticsearch:root

ENTRYPOINT ["/entrypoint.sh"]
