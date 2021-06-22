FROM node:current-alpine3.10

WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY package.json ./
COPY yarn.lock ./
RUN npm install
COPY src src
COPY public public

CMD npm start