FROM node:14-alpine

WORKDIR /app

RUN apk update && \
    apk add git && \
    npm install -g npm && \
    npm install -g vue-cli

COPY package*.json .

RUN npm install

COPY . .

EXPOSE 8080