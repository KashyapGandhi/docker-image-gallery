FROM node:21.6.2-alpine

ENV NODE_OPTIONS=--openssl-legacy-provider

WORKDIR /app

EXPOSE 3000

COPY package.json package-lock.json ./

RUN npm install --silent

COPY . ./

CMD ["npm", "start"]