# elastic-docker
3 node Elasticsearch cluster with Logstash, Kibana, Filebeat.

### Elastic Version

`7.4.0`

### Running

`docker-compose up`


### Sample Data

Upon startup, the following tasks are performed:

* Filebeat will ingest all log data from `./sample_data/elastic_blog_curated_access_logs`
* Logstash will import blog csv data from `./sample_data/blogs.csv`

This will yield the following indices:

* blogs
* logs_server1
* logs_server2
* logs_server3