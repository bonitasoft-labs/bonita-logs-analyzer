FROM docker.elastic.co/beats/filebeat:6.8.7

# Copy our custom configuration file
COPY filebeat.yml /usr/share/filebeat/filebeat.yml

USER root

VOLUME /usr/share/filebeat/logs