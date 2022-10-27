# Technologies-common-commands

Esse é um repositório para ajudar a lembrar os comandos de tecnologias mais utilizados de forma organizada

<br>

# Índice

## TECHS

### [Docker](#Docker)

### [Python](#PYTHON)

<BR>

# Docker

### Listar todos os containers ativos

<code>docker ps</code>

<hr/>

### Listar todos os containers (ativos e inativos)

<code>docker ps -a</code>

Imagens são uma receita para um container

<hr/>

### Listar todas as imagens

<code>docker images</code>

<hr/>

### Listar todos os containers ativos forma 2

<code>docker container ls</code>

<hr/>

### Listar todos os containers (ativos e inativos)

<code>docker container ls -a</code>

<hr/>

### Lista somente os ids de todos os containers ativos e inativos

<code>docker container ls -aq</code>

<hr/>

### Remover container (pode ser por id ou name)

<code>docker container rm dd8 1b0</code>

<hr/>

### Remover todos os containers

<code>docker container rm $(docker container ls -aq)</code>

<hr/>

### Listar somente o id de todas as imagens

<code>docker images -aq</code>

<hr/>

### Remover todas as imagens

<code>docker container rm $(docker images -aq)</code>

<hr/>

### Criar imagem a partir do dockerhub

<code>docker pull postgres</code>

<hr/>

### Criar e executar um container de postgres

<code>docker run --name t11-postgres -e POSTGRES_USER=chan -e POSTGRES_PASSWORD=1234 -d -p 5433:5432 postgres</code>

<hr/>

### Entra no bash de um container ativo

<code>docker exec -it id_do_container bash</code>

<hr/>

### Se conectar ao postgres do container usando o postgres de fora (sua máquina local)

<code>psql -h localhost -p 5433 -d nome_do_banco -U chan --password</code>

<hr/>

<br>

# PYTHON

## Verifica a versão do Python instalada

<code>python --version</code>

<hr/>

## Instala avaliador de más praticas

<code>pip install pycodestyle</code>

<hr/>

## Instala o pacote <nome_do_pacote>

<code>pip install nome-do-pacote</code>

<hr/>

## Desinstala o pacote <nome_do_pacote>

<code>pip uninstall -y nome-do-pacote</code>

<hr/>

## Lista todos os pacotes instalados no ambiente

<code>pip list</code>

<hr/>

## Mostra a versão de todos os pacotes instalados no ambiente

<code>pip freeze</code>

<hr/>

## Cria o ambiente virtual no diretório

<code>python -m venv venv</code>

<hr/>

## Ativa o ambiente virtual no diretório (WINDOWS)

<code>venv/Scripts/activate</code>

<hr/>

## Desativar o ambiente virtual no diretório(WINDOWS)

<code>deactivate</code>

<hr/>

## Criar o arquivo Requirements.txt

<code>pip freeze > requirements.txt</code>

<hr/>

## Instala os pacotes do arquivo Requirements.txt

<code>pip install -r requirements.txt</code>

<hr/>

## Lê os apps e transforma em migrations

<code>python manage.py makemigrations</code>

<hr/>

## Executa a migration para o Banco de Dados

<code>python manage.py migrate</code>

<hr/>

## Entra na shell do django do projeto

<code>python manage.py shell</code>

<hr/>

## Instala outra shell de python de melhor visual e sugestoes

<code>pip install ipython</code>

<hr/>

## Roda o servidor da aplicação

<code>python manage.py runserver</code>

<hr/>

## Instala o bug tracer IPDB

<code>pip install ipdb</code>

<hr/>

## Instala o motor engine para linkar o postgres à aplicação

<code>pip install psycopg2-binary</code>

<hr/>

## Instala o dotenv para puxar as variaveis de ambiente para a aplicação

<code>pip install python-dotenv</code>

<hr/>
