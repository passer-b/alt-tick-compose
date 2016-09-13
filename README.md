# alt-tick-compose

Alternative way to compose TICK stack by docker.  
  
InfluxData official repository is [here](https://github.com/influxdata/TICK-docker)

## About TICK stack

see [here](https://www.influxdata.com/get-started/what-is-the-tick-stack/)

## About Grafana

see [here](http://grafana.org/)

## Included services

- InfluxDB
- Telegraf
- Chronograf
- Kapacitor
- Grafana (you can use it instead of Chronograf)

Use official alpine linux image as much as possible.  
TICK stack use v0.13 image.  
Grafana use latest image.  

## Requirements

- Docker Engine 1.10.0 or above
- Docker Compose 1.6.0 or above

## Installation


``` bash
git pull https://github.com/passer-b/alt-tick-compose.git
```

## Usage


``` bash
docker-compose up

docker-compose down
```

If you want to learn more usage, see [docker-compose documents](https://docs.docker.com/compose/reference/).

## Configuration

TBD

## Directories

```
.
├── README.md                // this document
├── chronograf
│     ├── chronograf        // Chronograf data dir
│     └── chronograf.conf   // Chronograf config
├── docker-compose.yml       // Docker Compose config
├── grafana
│     ├── grafana           // Grafana data dir
│     └── grafana.ini       // Grafana config
├── influxdb
│     ├── influxdb          // InfluxDB data dir
│     └── influxdb.conf     // InfluxDB config
├── kapacitor
│     ├── kapacitor         // Kapacitor data dir
│     └── kapacitor.conf    // Kapacitor config
└── telegraf
       ├── telegraf.conf     // Telegraf config
       └── telegraf.d        // Telegraf config dir
```
