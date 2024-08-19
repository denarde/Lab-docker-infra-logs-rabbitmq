FROM fluent/fluentd:v1.14-debian-1

USER root

# Instala o plugin RabbitMQ para Fluentd
RUN gem install fluent-plugin-rabbitmq --no-document

USER fluent
