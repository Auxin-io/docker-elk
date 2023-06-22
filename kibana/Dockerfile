ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/kibana/kibana:8.2.0

RUN ls -al

COPY ./kibana/config/kibana.yml /usr/share/kibana/config

RUN pwd

WORKDIR config

RUN cat kibana.yml

RUN ls

# Add your kibana plugins setup here
# Example: RUN kibana-plugin install <name|url>
