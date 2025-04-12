# CP2 - Questão 6: Microserviço com Docker

Este projeto contém um microserviço simples em Python (`app.py`) que retorna mensagens na rota `/status`.

## Como Executar o Projeto

### Pré-requisitos
- Docker instalado

### Comandos Docker

#### a) Criar a imagem Docker
```bash
docker build -t meu-microservico .

#### b) Executar o container
```bash
docker run -d -p 5000:5000 --name microservico meu-microservico

#### c) Acessar o terminal do container
```bash
docker exec -it microservico bash

#### d) Verificar se o container está ativo
```bash
docker ps

#### e) Testar a aplicação
```bash
curl http://localhost:5000/
curl http://localhost:5000/status
