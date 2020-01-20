# IoT Docker

## Issues:

- in general seems like containers can't communicate between each other
- - node-red can't connect to mosquitto log error: `Connection failed to broker: mqtt://localhost:1883`
- - chronograf - it opens fine under `http://localhost:8888/` but once you try to connect it to influxdb `http://localhost:8086` it returns error

#### docker-compose including:

- [x] node-red
- [x] mosquitto
- [x] influxdb
- [x] chronograf (for influx)
- [x] telegraf (for influx)
- [x] grafana

#### Start / Stop / Logs

- `./start.sh`
- `./stop.sh`
- `./log.sh`

#### Utils

- `docker container kill $(docker ps -q)` kill all running containers

#### interesting links

- https://github.com/nicolargo/docker-influxdb-grafana
- https://github.com/jkehres/docker-compose-influxdb-grafana
