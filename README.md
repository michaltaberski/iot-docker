# IoT Docker

## Issues:

- in general seems like containers can't communicate between each other
- - node-red can't connect to mosquitto log error: `Connection failed to broker: mqtt://localhost:1883`
- - chronograf - it opens fine under `http://localhost:8888/` but once you try to connect it to influxdb `http://localhost:8086` it returns error

#### Start / Stop / Logs

- `./start.sh`
- `./stop.sh`
- `./log.sh` or `docker-compose logs -f nginx`

#### Utils

- `docker container kill $(docker ps -q)` kill all running containers

#### interesting links

- https://github.com/nicolargo/docker-influxdb-grafana
- https://github.com/jkehres/docker-compose-influxdb-grafana
