# Pipeline de Logs do Nginx com Fluentd, RabbitMQ, Logstash, Elasticsearch e Kibana

## Visão Geral

Este laboratório configura um pipeline completo de logs utilizando Docker. O ambiente captura logs de um servidor Nginx, processa-os através do Fluentd, envia-os para o RabbitMQ, e depois consome e armazena os logs no Elasticsearch usando o Logstash. Finalmente, o Kibana é utilizado para visualizar e analisar os logs.

### Componentes:

1. **Nginx**: Um servidor web que gera logs.
2. **Fluentd**: Um coletor de dados que captura os logs do Nginx e os envia para o RabbitMQ.
3. **RabbitMQ**: Um broker de mensagens que armazena os logs antes do processamento.
4. **Logstash**: Uma ferramenta de processamento de logs que consome os logs do RabbitMQ e os envia para o Elasticsearch.
5. **Elasticsearch**: Um motor de busca e análise que armazena e indexa os logs.
6. **Kibana**: Uma ferramenta de visualização que permite explorar os logs armazenados no Elasticsearch.

## Pré-requisitos

- Docker e Docker Compose instalados no sistema.