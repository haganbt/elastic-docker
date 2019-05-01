# elastic-docker
My Elastic stack setup using docker compose. Elasticsearch, Logstash, Kibana.

### Version: 6.5.4

### Running

`docker-compose up`

NOTE: as default, no ES data is persisted. To persist data, uncomment the appropriate `volume` within `docker-compose.yaml`.