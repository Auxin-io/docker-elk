ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:8.2.0

USER root

COPY . /

RUN ls
RUN pwd
WORKDIR /setup
RUN ls
RUN pwd
RUN set -eux
RUN	mkdir /state
RUN	chown elasticsearch /state
RUN	chmod +x /entrypoint.sh

USER elasticsearch:root

ENTRYPOINT ["/entrypoint.sh"]
