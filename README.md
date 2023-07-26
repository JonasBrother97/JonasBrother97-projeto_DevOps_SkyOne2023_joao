# Desafio DevOps - Docker

Este repositório contém uma configuração Docker para executar o Desafio DevOps - Docker.

**Acesse a aplicação em `http://localhost:8000/polls` após executar o contêiner.**

## Pré-requisitos

Docker: Certifique-se de ter o Docker instalado em sua máquina. Você pode baixá-lo [aqui](https://www.docker.com/get-started).

## Como usar

[Docker](https://github.com/JonasBrother97/projeto_DevOps_SkyOne2023_joao/tree/main#pull-from-docker-hub) | [Docker Compose](https://github.com/JonasBrother97/projeto_DevOps_SkyOne2023_joao/tree/main#docker-compose) | [Build docker locally](https://github.com/JonasBrother97/projeto_DevOps_SkyOne2023_joao/tree/main#build-docker-locally)

### Docker

```bash
docker pull flatbed7044/skyone_jg_image:latest
```

``` bash
docker run -d -p 8000:8000 flatbed7044/skyone_jg_image:latest
```

### Docker Compose

Necessário ter o docker-compose instalado em sua máquina. Você pode baixá-lo [aqui](https://docs.docker.com/compose/install/).

Utilize o arquivo [docker-compose.yml](https://github.com/JonasBrother97/projeto_DevOps_SkyOne2023_joao/blob/main/docker-compose.yml) como exemplo e execute o seguinte comando:

```bash
docker-compose up -d
```

### Build docker locally

Siga os passos abaixo para executar o Desafio DevOps - Docker usando o Docker:

1. Clone este repositório:

```bash
git clone https://github.com/JonasBrother97/projeto_DevOps_SkyOne2023_joao.git
```

2. Navegue até o diretório do projeto:

```bash
cd projeto_DevOps_SkyOne2023_joao/mysite
```

3. Construa a imagem Docker:

```bash
docker build -t mysite .
```

4. Execute o contêiner Docker:

```bash
docker run -d -p 8000:8000 mysite
```