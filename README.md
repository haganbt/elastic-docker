# elastic-docker
Elasticsearch, Logstash, Kibana, Filebeat.

### Version

`6.5.4`

### Running

`docker-compose up`


### Sample Data

Upon startup, the following tasks are performed (see the `./sample_data` folder):

* Filebeat will ingest all log data from `./sample_data/elastic_blog_curated_access_logs`
* Logstash will import blog csv data from `./sample_data/blogs.csv`

This will yield the following indices:

* blogs
* logs_server1
* logs_server2
* logs_server3

WARNING: as default, no ES data is persisted. To persist data, uncomment the appropriate `volume` within `docker-compose.yaml`.