ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:8.2.0

RUN ls -al

RUN pwd

COPY ./elasticsearch/config/elasticsearch.yml /usr/share/elasticsearch/config

WORKDIR config
RUN ls

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
