Comandos docker

/testes:
docker build -t testenodeteste .
docker run --network test-network testenodeteste

/main-app:
docker build -t testenode .
docker run -d --name app --network test-network testenode

Network:
docker network create test-network
