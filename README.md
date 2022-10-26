# Technologies-common-commands

Esse é um repositório para ajudar a lembrar os comandos e tecnologias mais utilizados de forma organizada

<br>

# Docker

## Listar todos os containers ativos

docker ps

<hr/>

## Listar todos os containers (ativos e inativos)

docker ps -a

Imagens são uma receita para um container

<hr/>

## Listar todas as imagens

docker images

<hr/>

## Listar todos os containers ativos forma 2

docker container ls

<hr/>

## Listar todos os containers (ativos e inativos)

docker container ls -a

<hr/>

## Lista somente os ids de todos os containers ativos e inativos

docker container ls -aq

<hr/>

## Remover container (pode ser por id ou name)

docker container rm dd8 1b0

<hr/>

## Remover todos os containers

docker container rm $(docker container ls -aq)

<hr/>

## Listar somente o id de todas as imagens

docker images -aq

<hr/>

## Remover todas as imagens

docker container rm $(docker images -aq)

<hr/>

## Criar imagem a partir do dockerhub

docker pull postgres

<hr/>

## Criar e executar um container de postgres

docker run --name t11-postgres -e POSTGRES_USER=chan -e POSTGRES_PASSWORD=1234 -d -p 5433:5432 postgres

<hr/>

## Entra no bash de um container ativo

docker exec -it id_do_container bash

<hr/>

## Docker - Se conectar ao postgres do container usando o postgres de fora (sua máquina local)

psql -h localhost -p 5433 -d nome_do_banco -U chan --password

<hr/>
