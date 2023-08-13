# Dockerizar Elasticsearch
Dockerizar elasticsearch, filebeat, kibana, logstash

## Archivos de configuracion

- Elasticsearch ruta: ./elasticseach/config
- Logstash ruta: ./logstash/settings/
- Filebeat ruta: ./filebeat-docker/

## Ruta desde va leer los archivos wildfly
 - En archivo docker-compose.yml ir al apartado de volumenes de filebeat, y modificar el path con la ruta donde se encuentren los log ejemplo: ```- ruta-local-donde-estan-logs:/usr/share/filebeat/log-generatorg``` 

## Crear y correr el contenedor 

```docker compose up -d```


## Borrar el contenedor stop al contenedor 

```docker compose down```


## Kibana 
- Nota: esperar unos minutos para que carguen todos los servicios.
- Entrar en la siguiente para ver manage de Kibana
[localhost:5601](http://localhost:5601/)

## Generar logs de pruebas 

dentro de la carpeta logs ejecutar 
```  java -jar .\log-generator-1.0.jar -l 100 -d 1000 ```


<img src="./kibana.png" alt="MDN" />