# prometheus-and-grafana
Sample application on how to monitor spring boot application using actuator, prometheus and grafana dashboard.

## setup prometheus in docker
>Follow the steps
- run the following command in after starting docker instance to pull imnage
``` 
 docker pull prom/prometheus:latest
 ``` 
- create prometheus.yml config file for prometheus server as available in this project
- run following command to docker prometheus
```
docker run -v C:\path\prometheus.yml:/etc/prometheus/prometheus.yml -p  9090:9090 prom/prometheus:latest
```

>**Note:** IP address in prometheus.yml file should be local ip instead of 'localhost' because we are using docker
