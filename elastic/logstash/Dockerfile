FROM docker.elastic.co/logstash/logstash:6.8.7

RUN rm -f /usr/share/logstash/pipeline/logstash.conf
COPY pipeline /usr/share/logstash/pipeline/
