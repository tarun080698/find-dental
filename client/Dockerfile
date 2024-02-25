# step 1: fetching node image
FROM node:18-alpine as build

WORKDIR /client/

COPY public/ /client/public
COPY src/ /client/src
COPY package.json /client/

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "run", "start"]