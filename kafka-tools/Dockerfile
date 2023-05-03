FROM  confluentinc/cp-enterprise-kafka:7.3.3

USER root
# Set up a user to run Kafka
RUN groupadd kafka && \
  useradd -d /kafka -g kafka -s /bin/false kafka && \
  chown -R kafka:kafka /usr/bin/

USER kafka
ENV PATH /usr/bin:$PATH
WORKDIR /usr/bin
