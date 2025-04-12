# CP2 - Questão 6: Microserviço com Docker

Este projeto contém um microserviço simples em Python (`app.py`) que retorna mensagens na rota `/status`.

## Como Executar o Projeto

### Pré-requisitos
- Docker instalado

### Comandos Docker

### a) Criar a imagem Docker

docker build -t meu-microservico .

### b) Executar o container

docker run -d -p 5000:5000 --name microservico meu-microservico

### c) Acessar o terminal do container

docker exec -it microservico bash

### d) Verificar se o container está ativo

docker ps

### e) Testar a aplicação

curl http://localhost:5000/

curl http://localhost:5000/status
