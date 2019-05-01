# elastic-docker
Elasticsearch, Logstash, Kibana with sample data loaded from a local csv file using Logstash.

### Version

`6.5.4`

### Running

`docker-compose up`

NOTE: as default, no ES data is persisted. To persist data, uncomment the appropriate `volume` within `docker-compose.yaml`.