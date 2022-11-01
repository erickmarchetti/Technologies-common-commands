# Technologies-common-commands

Esse é um repositório para ajudar a lembrar os comandos de tecnologias mais utilizados de forma organizada

<br>

<a id="indice"></a>

# Índice

### [Docker](#Docker)

### [Python](#Python)

### [Criando do 0 com Django](#projetoDjango1)

<br>

<a id="Docker"></a>

<details>
    <summary style="font-size: 18px">Docker:</summary>

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

### Criar image apartir de um dockerfile

<code>docker build -t image_name .</code>

<hr/>

</details>

<br>

<a id="Python"></a>

<details>
    <summary style="font-size: 18px">Python:</summary>

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

## Ativa o ambiente virtual no diretório

<code>venv/bin/activate</code> (Linux)

<code>venv/Scripts/activate</code> (Windows)

<hr/>

## Desativar o ambiente virtual no diretório

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

<br/>

## Instala o drf-spectacular para criação da documentação da aplicação

<code>pip install drf-spectacular</code>

<hr/>

## Cria o projeto em Django

<code>django-admin startproject nome-do-projeto .</code>

<hr/>

## Cria app no projeto em Django

<code>python manage.py startapp nome-do-apps</code>

<hr/>

## Conectar ao postgreSQL

<code>psql -U nome-do-banco</code>

<hr/>

## Cria Super User na shell do projeto

<code>./manage.py createsuperuser</code>

<hr/>
</details>

<br>

<a id="projetoDjango1"></a>

<details>
    <summary style="font-size: 18px">Projeto com Django do 0</summary>
<br>

### Passo a passo para criar do zero

<code>1) Clone o repositório forkado para sua máquina local;</code>
<br>
<code>1) Entre nele;</code><br>
<code>2) Crie seu ambiente virtual; (python -m venv venv)</code><br>
<code>3) Ative o ambiente virtual; (source venv/scripts/activate)</code><br>
<code>4) Instale os pacotes referentes ao Django Rest Framework;</code><br>
<code>5) Crie um arquivo requirements.txt com as dependencias do projeto;</code><br>
<code>6) Crie um arquivo .gitignore e ignore os arquivos necessários;</code><br>
<code>7) Crie o projeto principal (django-admin startproject nome do projeto .)</code><br>
<code>8) Entre no urls.py do projeto e coloque o include no import do url</code><br>
<code>9) Entre no settings.py e faça as alterações devidas nos apps</code><br>
<code>10) Customize a Model de user</code><br>
<code>11) Instale a model customizada nos apps de settings.py</code><br>
<code>12) Rode a primeira migration</code><br>
<code>13) Faça a serializer de user</code>

<hr/>
</details>
<br/>

### [Índice](#indice)
