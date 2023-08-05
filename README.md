# Oficina Markdown + HTML

Workshop desenvolvido para [CAMARADES Brasil](https://camaradesbrasil.bio.br/) por [vyk1](https://github.com/vyk1/)

## Markdown

Desenvolvido usando [@marp-team/marp-cli](https://github.com/marp-team/marp-cli) com [Docker](https://hub.docker.com/r/marpteam/marp-cli/).

> Há um Dockerfile disponível, caso uses docker compose

### Para dar build:
`docker build -t marp-app .`

### Para executar e servir:
`docker run --rm --init -v ${PWD}:/home/marp/app/ -e LANG=$LANG -p 8080:8080 marp-app -s`

### Para acessar:
http://localhost:8080/

### Dentro do container, converta para HTML, usando:
`marp-app md/index.md`

### Para converter para PDF:
`marp-app md/index.md --pdf`

### Para servir com Python 3:
`cd html`
`python3 -m http.server 8080`

## HTML

Acessar normalmente com seu navegador de preferência.

