FROM docker.elastic.co/logstash/logstash:7.1.1
RUN rm -f /usr/share/logstash/pipeline/logstash.conf
RUN mv /usr/share/logstash/config/logstash-sample.conf /usr/share/logstash/logstash-sample.conf
RUN mkdir /usr/share/logstash/input/
ADD input/ /usr/share/logstash/input/
ADD config/ /usr/share/logstash/config/

