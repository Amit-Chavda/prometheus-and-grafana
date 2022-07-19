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

- Open the localhost:9090 and you will see dashboard similar like this

### Prometheus query engine
![image](https://user-images.githubusercontent.com/47694676/179746219-97df457c-f8f9-4abe-8291-27f0f1da4fcf.png)

### Grafana Dashboard for Spirng Boot Application
![image](https://user-images.githubusercontent.com/47694676/179804077-6373505b-4117-463c-ae55-80d559d60340.png)
>Import [this code](https://github.com/Amit-Chavda/prometheus-and-grafana/blob/b476fc8ed6eb1630db5f2953ac51af51a848b9bb/Spring%20Boot%20Statistics.json) in grafana for similar dashboard.
