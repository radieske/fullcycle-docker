FROM node:15

WORKDIR /usr/src/app

ENV DOCKERIZE_VERSION=v0.7.0

RUN wget -O - https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz | tar xzf - -C /usr/local/bin \
    && apt-get autoremove -yqq --purge wget && rm -rf /var/lib/apt/lists/*

# o docker vai copiar todos os arquivos e pastas do diretorio atual 
# para o diretorio /usr/src/app

EXPOSE 3000

# CMD ["node", "index.js"]