FROM node:15

WORKDIR /usr/src/app

COPY . .
#instalando o npm
RUN npm install

RUN npm install --save express

RUN apt-get update && apt-get install -y wget

ENV DOCKERIZE_VERSION v0.6.1

RUN wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && tar -C /usr/local/bin -xzvf dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && rm dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz
#propriedades do shell para iniciar a instalação
CMD["npm","run","start"]

EXPOSE 3000
