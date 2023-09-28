# Docker-Swarm


docker swarm init

docker build -t nodeyo .

docker stack deploy -c docker-compose.yml service-node

el primer comando activa swarm en el dispositivo.

el segundo toma el servidor pequeño y lo hace una imagen llamada nodeyo para luego ser utilizada por el tercer comando.

el tercer comando crea el servicio donde "docker-compose.yml" es el nombre del archivo que contiene la configuracion y "service-node" es el nombre que le doy al mismo.
Una vez finalizado los comandos, puede aumentar o disminuir la cantidad de servicios con el siguiente comando:

docker service scale service_node_web=5
en el codigo anterior crea 5 servicios, puede poner la cantidad que quiera cambiando el valor del mismo.
