# prometheus-grafana-spring boot

![cover](https://miro.medium.com/max/1200/1*sI4Zz0bhktt9eZ3sq2oLdg.jpeg)

prometheus-grafana-spring boot

A simple example for a Prometheus and Grafana Monitoring setup with an example spring boot backend exposing metrics.

## Run the System
We can easily run the whole with only a single command:
```bash
docker-compose up
```

The services can be run on the background with command:
```bash
docker-compose up -d
```

## Stop the System
Stopping all the running containers is also simple with a single command:
```bash
docker-compose down
```

If you need to stop and remove all containers, networks, and all images used by any service in <em>docker-compose.yml</em> file, use the command:
```bash
docker-compose down --rmi all
```

`./docker/docker-compose.yml`
- starts prometheus and grafana

`./docker/data/`
- contains data for grafana and prometheus

See `docker/data/prometheus/config/prometheus.yml` for the prometheus configuration and change the target to your IP address to enable scraping metrics for your locally running service.