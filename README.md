# Prometheus Hackathon

## prerequisites
  - Docker


follow the below steps to set up hackathon environment

  - clone this repo and run `docker compose up` from the project folder
  - check the following endpoints are accessible 
     - http://localhost:9090/metrics
     - http://localhost:9100/metrics
     - http://localhost:8080/metrics
  
use http://localhost:3000 to access gradana. default username and password admin is admin 

## task
 - create a new  data source of prometheus in grafana, refer: (https://grafana.com/docs/grafana/latest/datasources/prometheus/configure-prometheus-data-source/)
 - create a dashboard based on following metrics
    - `container_memory_max_usage_bytes`, create a chart to count maximum memory usages of each container
    - `promhttp_metric_handler_requests_total` create a chart to count the status of requests (200, 404 etc)
    - `prometheus_http_requests_total` create a chart to count the endpoints
    - `process_cpu_seconds_total` using this metrics create a chart of cpu usage of each container

