# Containers
- pacote de código que pode executar alguma ação (baseado na imagem)
  - um container não roda sem uma imagem
  - imagem tem projeto do container
  - conteiner é a execução de fato
- cada tec tem seu container
- os projetos são executados dentro dos containers que criamos / utilizamos
- multiplos containers rodam juntos

## Container x Imagem
- imagem
  - projeto que será executado
    - comandos
    - arquivos que vão iniciar app
    - portas exportas
    - uma imagem pode ter outra imagem de base
  - programamos uma imagem e excutamos por meio de um container

## Onde encontrar imagens
- [site oficial](https://hub.docker.com/)
  - onde verificamos quais imagens existem na documentação oficial e como utiliza-las

# Container x VM (Virtual machine)
- Container é aplicação qeu serve para um determinado fim, não possui sistema operacional
  - seu tamanho é alguns mbs (menos que um sistema operacional)
  - gastam menos recursos para serem executados por causa do seu uso específico

- VM possui sem próprio sistema operacional próprio
  - seu tamanhoa é de gbs
  - Gastam mais recursos porém pode executar diversas funções ao mesmo tempo