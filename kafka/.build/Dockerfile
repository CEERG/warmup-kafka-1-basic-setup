FROM openjdk:11

RUN wget https://dlcdn.apache.org/kafka/3.1.0/kafka_2.13-3.1.0.tgz
RUN	tar -xzf kafka_2.13-3.1.0.tgz

WORKDIR /kafka_2.13-3.1.0

COPY server.properties config
COPY consumer.properties config

ENTRYPOINT bin/kafka-server-start.sh config/server.properties