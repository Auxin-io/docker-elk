ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:8.2.0

USER root

COPY . /

RUN set -eux
RUN	mkdir /state
RUN	chown elasticsearch /state
WORKDIR /setup
RUN ls -la
RUN pwd


USER elasticsearch:root

ENTRYPOINT ["/entrypoint.sh"]
