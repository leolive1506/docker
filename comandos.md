# Executar uma imagem
  - cria um novo container
```sh
# docker run docker/whalesay cowsay Hello_word
docker run <imagem>
```
# Deixar em execução
  - assim podemos executar comandos disponiveis no container
```sh
docker run -it <imagem>
```
# Roda container em background (detached)
  - não ocupa aba no terminal
```sh
docker run -d <imagem>
```
# ver containers que estão rodando
```sh
docker ps
# ou
docker container ls

# container estão rodando e já foram executados
docker ps -a
```
# Voltar a utilizar um container de onde parou
  - se existirem processos continua
```sh
docker start <id>
```
# stop container
```sh
docker stop name_in_list_docker_ps_or_id
```

# Expor portas
- container é isolado e não tem conexão com nada de fora deles
- expor portas a flag é **-p**
  - -p 80:80
  - porta_pc:porta_container
```sh
docker run -d -p 80:80 nginx
docker run -d -p 3000:80 nginx
```

# Definir o nome
  - se não definir, recebe nomes aleatorios
```sh
docker run -d -p 80:80 --name nginx_app nginx
```

# Verificar logs
```sh
docker logs <id>
# deixar aberto arquivo de logs
docker logs -f <id>
```

# Remover containers
```sh
docker rm <id>
# -f (force) se ainda estiver em execução
docker -rm -f <id>
```