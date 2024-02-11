FROM node:20-alpine

RUN mkdir -p /app/src

WORKDIR /app/src

COPY package*.json ./

RUN npm install

COPY dist/server.js ./

# import env variables here using ENV <header> <value>

EXPOSE 3003

CMD [ "npm", "start" ]
