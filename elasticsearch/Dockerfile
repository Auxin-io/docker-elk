ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:8.2.0

COPY ./elasticsearch/config/elasticsearch.yml /usr/share/elasticsearch/config

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
