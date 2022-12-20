# FULLCYCLE: DESAFIO 1: GOLANG

Este é o código desenvolvido para o primeiro desafio do módulo Docker do curso Full Cycle. O objetivo é criar uma imagem que rode um executável que exiba a mensagem `Full Stack Rocks!!` desenvolvido em GoLang. A imagem deve ter no máximo 2Mb e deve estar disponível no dockerhub.

## Usando o código-fonte

Após clonar o projeto, navegue pelo terminal até a pasta com os arquivos e faça o `build` da imagem

```bash
docker build -t fullcycle-go . -f Dockerfile
```

Em seguida, rode o container com a imagem que acabou de criar

```bash
docker run --name fullcycle-go -v $(pwd):/src fullcycle-go:latest
```

Você deve receber a mensagem `Full Cycle Rocks!!` em seu terminal

## Usando a imagem no dockerhub

Para usar a imagem hospedada no dockerhub, basta usar o seguinte comando:

```bash
docker push stsmuniz/fullcycle:latest
```

Você deve receber a mensagem `Full Cycle Rocks!!` em seu terminal