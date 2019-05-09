# docker-compose-elasticsearch-kibana

# Overview

Docker Compose for 3 Node Elasticsearch (7.0.1) Cluster and Kibana (7.0.1) Instance for development purpose.

- [x] 3 Node Elasticsearch version 7.0.1
- [x] Kibana version 7.0.1
- [x] NGINX

# NOTES

- We use Open Source version. If you need to change to standard version please change to elasticsearch and kibana respectively.
- Kibana is being served behind Nginx Proxy

### Start Stack

```
docker-compose up -d
```

### Check status of docker-compose cluster

```
docker-compose ps
```

### Stop Stack

```
docker-compose down
```

### Cluster Node Info

```
curl http://localhost:9200/_nodes?pretty=true
```

### Access Kibana

```
http://localhost:5601
```

### Accessing Kibana through Nginx

```
http://localhost:8081
```

### Access Elasticsearch

```
http://localhost:9200
```

### List docker volume

```
docker volume ls
```

### Remove unuse docker volume

```
docker volume prune
```
