# Dockerizar Elasticsearch
Dockerizar elasticsearch, filebeat, kibana, logstash

## Configuration files

- Elasticsearch ruta: ./elasticseach/config
- Logstash ruta: ./logstash/settings/
- Filebeat ruta: ./filebeat-docker/

## Path files wildfly
 - En archivo docker-compose.yml ir al apartado de volumenes de filebeat, y modificar el path con la ruta donde se encuentren los log ejemplo: ```- ruta-local-donde-estan-logs:/usr/share/filebeat/log-generatorg``` 

## Create and run the container 

```docker compose up -d```


## Stop y delete container 

```docker compose down```


## Kibana 
- Nota: wait a few minutes while all services are loaded.
- Enter in the following url manage de Kibana
[localhost:5601](http://localhost:5601/)


<img src="./kibana.png" alt="MDN" />