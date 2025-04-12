# CP2 - Questão 6 
O código do app.py retorna mensagens na rota /status.

 Crie os comandos necessários para: 
a) Criar a imagem Docker chamada meu-microservico.
docker build -t meu-microservico .

 b) Rodar o container expondo a porta correta.
docker run -d -p 5000:5000 --name microservico meu-microservico

 c) Acessar o terminal do container.
docker exec -it microservico bash

 d) Verificar se o container está ativo.
docker ps

 e) Testar se a aplicação está funcionando via terminal.
 curl http://localhost:5000/
 curl http://localhost:5000/status