# Introdução ao Docker
<img align="right" width=35% src="assets/docker.png">

### O que é o Docker ?

<font size=3> O Docker é um conjunto de Softwares, que utiliza **virtualização a nivel  de SO**<sup>[1]</sup> para criação de ambientes isolados(Containers) para execução de Software de maneira que independentemente da maquina ele seja executado sempre em um ambiente identico com as mesmas bibliotecas, software e Sistema Operacional.

### Como ele funciona ?

De maneira simplificada podemos dividir o docker em 4 blocos que definem sua arquitetura :
- **Docker Client:** A principal parte que o desenvolvedor interage, aqui estão os comandos como o docker run, build e pull. Utiliza a API Docker para se comunicar com o **Daemon**<sup>[2]</sup> Docker, podendo interagir tambem com Daemons remotos.
- **Docker Daemon:** É responsavel por receber as requisições da API docker e administrar os objetos Docker tais quais imagens, containers, redes e volumes. Além disso ele pode se comunicar com outros *daemons*
- **Docker Registry:** É onde ficam armazenadas as imagens Docker, o principal registro publico é o [Docker hub](https://hub.docker.com/), sempre que utilizamos o `docker run` ou `docker pull` ele busca a imagem nos seus registros configurados, por padrão o DockerHub. <br> 
***Nota:*** Voce pode criar Registros privados para armazenar suas imagens customizadas.
- **Docker Objects:** São os componentes utilizados pelo docker: Imagens, volumes de armazenamento, containers, redes e plugins. <br>
***Nota:*** Mais a frente os conceitos de imagens, volumes e containers serão mais aprofundados

<img src="assets/docker-architecture.webp" alt="Diagrama que exemplifica a arquitetura do docker">

### Como instalar o Docker ?

A documentação do docker explica de maneira detalhada como instalar no Windows, MacOs e linux, basta seguir os passos no site de acordo com seu SO.

### [Install Docker | Docker docs](https://docs.docker.com/engine/install/)

Caso queria testar o docker sem a necessidade de instalar-lo em sua maquina a ferramenta PlayWithDocker pode ser usada gratuitamente diretamente do seu navegador 
### [Play with Docker](https://labs.play-with-docker.com/)

## Referencia e Links uteis

1. [Virtualização a Nivel de SO - Wikipedia](https://pt.wikipedia.org/wiki/Virtualiza%C3%A7%C3%A3o_em_n%C3%ADvel_de_sistema_operacional)
2. [Daemon (computação) - Wikipedia](https://pt.wikipedia.org/wiki/Daemon_(computa%C3%A7%C3%A3o))
---
- [Docker Overview - Docker docs](https://docs.docker.com/get-started/overview/)
- [O que é virtualização - RedHat](https://www.redhat.com/pt-br/topics/virtualization/what-is-virtualization)
