# dockerizar-elasticsearch
Dockerizar elasticsearch, filebeat, kibana, logstash

## Crear y correr el contenedor 

```docker compose up```


## Borrar el contenedor stop al contenedor 

```docker compose down```


## Kibana 

[localhost:5601](http://localhost:5601/)

## Generar logs de pruebas 

dentro de la carpeta logs ejecutar 
```  java -jar .\log-generator-1.0.jar -l 100 -d 1000 ```
