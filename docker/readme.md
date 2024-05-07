Docker

docker ps -a -q
vai listar somente os id's

docker rm $(docker ps -a -q) -f
vai apagar todos os containers até os que estão rodando

ENTRYPOINT
sempre fixo
![alt text](image-1.png)

CMD
variável que entra como um parâmetro do entrypoint
![alt text](image.png)

EXPOSE 80
isso significa que eu estou deixando a porta 80 do meu container exposta

Network
Para fazer um container se conectar com o outro
bridge para um container se comunicar com o outro
host mescla a network do docker com a network do host do docker
overlay para quando tem vários docker em várias redes se conectarem
maclan para simular uma network conectada na minha rede
none para não ter nenhuma rede e rodar de forma totalmente isolada

Network Bridge
docker network inspect bridge = inspecionar a network

docker attach (nomedocontainer)
ip add show = o próprio ip do container
ping (ip do outro container)

docker network create --driver brigde nomeDaRede
docker run -dit --name nomeDoPrimeiroContainer --network nomeDaRede bash
docker run -dit --name nomeDoSegundoContainer --network nomeDaRede bash

docker exec -it nomeDoPrimeiroContainer bash = entrar dentro do container da network

ping nomeDoSegundoContainer = agora vai encontrar o segundo container

docker network connect nomeDaRede nomeDoTerceiroContainer

Network HOST
docker run --rm -d --name ngnix --network host ngnix

Bridge

docker ps - verificar quais containers estão ativos
docker ps -a = verificar todos os containers mesmo que inativos
-i = modo interativo para manter seu processo rodando e permitir digitação
-t = desacoplar o terminal do container
:latest = tag da imagem

docker start + nome do container ou id(completo ou parcial) = rodar o container
docker stop + nome do container ou id(completo ou parcial) = parar o container
–rm = rodar de modo que depois que o container parar ser removido
-p = publicar a porta para acessar (-p 8080:80) 8080 é a porta da máquina que vai ser referenciada e 80 é a porta do container
-d = detach rodar um container e deixar o terminal livre
docker rm + nome do container ou id(completo ou parcial) = remover o container
docker rm + nome do container ou id(completo ou parcial) - f = remover container mesmo que esteja rodando  
– name = inserir um nome para o container
docker exec = executa comando dentro do container

docker volume create nomedovolume
docker volume inspect nomedovolume

docker run –name nginx(imagem) -d –mount type=volume, source=nomedovolume, target=/app nginx
docker volume prune= vai parar tudo o que for de volume que não estiver sendo utilizado

Trabalhando com imagens - iniciar
docker images = mostra as imagens que está na sua máquina
docker rmi = remover a imagem

criando uma imagem
docker build -t nome do usuário do dockerHub/ nome da imagem: tag(definir versão ou usar o latest por padrão) . o ponto indicando que está na pasta atual

workdir = diretório que vou trabalhar dentro do container, vai criar a pasta com esse nome e me deixar dentro dela

&& concatenar comandos
\ quebrar linha

copy = copiar de dentro do meu computador para o docker

expose = exportar a porta do container
