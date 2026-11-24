# Trabalho-4-docker
Trabalho acadêmico - aplicação web com Docker
Runbook — Como executar o serviço

1. Pré-requisitos

* Docker Desktop instalado.
* Docker em funcionamento.
* Git para acessar o repositório.

2. Baixar o projeto

git clone LINK_DO_REPOSITORIO
cd Trabalho-4-docker

3. Construir a imagem

docker build -t trabalho-4-docker .

4. Iniciar o container

docker run -d --name trabalho-web -p 8080:80 --restart on-failure trabalho-4-docker

5. Testar a aplicação

Abrir o navegador e acessar:

http://localhost:8080

6. Verificar o container

docker ps

docker ps -a

7. Consultar logs

docker logs trabalho-web

8. Parar o serviço

docker stop trabalho-web

9. Remover o container

docker rm trabalho-web

Observação

Os comandos e procedimentos descritos neste roteiro deverão ser validados no ambiente Docker antes da demonstração. As limitações do ambiente de execução serão documentadas, se necessário.