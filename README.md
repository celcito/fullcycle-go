# Full Cycle Go App

Este repositório contém o código-fonte e o `Dockerfile` para uma aplicação Go simples que imprime "Full Cycle Rocks!!" quando executada. A aplicação é construída e empacotada em uma imagem Docker extremamente leve, utilizando a imagem base `scratch` para minimizar o tamanho final da imagem.

## Pré-requisitos

- Docker instalado na sua máquina.

## Construção da Imagem Docker

Para construir a imagem Docker, execute o seguinte comando no diretório raiz do projeto:

bash docker build -t celcito/fullcycle .


Este comando compila o código Go e cria uma imagem Docker a partir do `Dockerfile` presente neste repositório.

## Execução da Imagem Docker

Após construir a imagem, você pode executá-la usando o seguinte comando:

bash docker run celcito/fullcycle


Isso iniciará um contêiner a partir da imagem `celcito/fullcycle` e imprimirá "Full Cycle Rocks!!" no terminal.

## Publicação da Imagem no Docker Hub

Para publicar a imagem no Docker Hub, primeiro faça login no Docker CLI:


bash docker login


Em seguida, publique a imagem:

bash docker push celcito/fullcycle


## Acessando a Imagem no Docker Hub

Você pode acessar a imagem `celcito/fullcycle` no Docker Hub através do seguinte link:

[celcito/fullcycle](https://hub.docker.com/r/celcito/fullcycle)




## Rodando a Imagem a partir da imagem hospedada no  Docker Hub

Você pode rodar a imagem  com o comando.

docker run celcito/fullcycle


Isso fará com que a imagem seja baixarda e executada iniciando  um contêiner a partir da imagem `celcito/fullcycle` e imprimirá "Full Cycle Rocks!!" no terminal.

## Conclusão

Este projeto demonstra como criar uma aplicação Go simples, empacotá-la em uma imagem Docker extremamente leve usando a imagem base `scratch`, e publicá-la no Docker Hub. Isso é útil para cenários onde o tamanho da imagem é uma preocupação, como em ambientes de produção em nuvem ou em dispositivos IoT com recursos de memória limitados.