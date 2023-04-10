# prometheus-grafana
This is a sample repo for running prometheus and grafana in local

# Run using docker-compose 
```
docker-compose up
```

# Follow this steps once the containers are running
- Prometheus
    - Go to http://localhost:9090/
    - Go to status -> targets you should be able to see 2 targets -> node_exporter and prometheus
- Grafana
    - Go to http://localhost:3000/
    - Login with default username and password -> admin/admin
    - Setup the data source
        - Select Prometheus
        - Add HTTP url - http://prometheus:9090
    - Add new dashboard -> import or create yourselves.
