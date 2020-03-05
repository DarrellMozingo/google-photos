FROM node:13.8.0-slim

COPY package.json /app/package.json
COPY package-lock.json /app/package-lock.json

WORKDIR /app

RUN npm install

COPY . /app

CMD node app.js