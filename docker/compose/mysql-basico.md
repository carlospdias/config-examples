## Como usar o mysql-basico

Execute
```sh
$ docker-compose -f mysql-basico.yml  up

```
Verifica se não apresenta nenhum erro e então, 
Entre por esse link na tela administrativa
http://localhost:8090/

use as credenciais
 - usuário root
 - senha   password

## Limpeza de Ambiente Docker

```sh
#https://www.digitalocean.com/community/tutorials/how-to-remove-docker-images-containers-and-volumes

docker system prune -a
docker image prune
docker rmi $(docker images -a -q)
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
docker volume prune
```
