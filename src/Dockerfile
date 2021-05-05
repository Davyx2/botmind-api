ARG TAG=lts-alpine3.12

FROM  node:$TAG

RUN mkdir -p /usr/src/app && apk add curl

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY  . .

EXPOSE 8080

CMD ["npm", "prod"]
