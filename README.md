# Elasticsearch Dojo

## Summary

Elasticsearch Dojo is a docker compose file for creating a 3 node clustered Elasticsearch instance via docker. This includes Kibana and the head plugin for Elasticsearch. This is mainly for rapid development and working with an minimal but optimal setup requirements 
## Setup

Docker and docker-compose will need to be installed, as well as enough memory to operate all nodes. 4gb or greater will be needed.

### Memory management

To increase or decrease RAM used by an Elastic node edit the `environment` setting within the .yml file.

```
      - "ES_JAVA_OPTS=-Xms512m -Xmx512m"
```


## Usage

Within the directory of the compose.yml file

### Start

```
docker-compose up
```

### Stop

```
docker-compose stop
```

### Remove compose containers

```
docker-compose rm
```
