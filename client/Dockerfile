FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app
COPY package*.json ./
COPY public public
COPY vite.config.js vite.config.js
COPY index.html index.html
# COPY .eslintrc.cjs .eslintrc.cjs
RUN npm i
COPY src src
EXPOSE 5173
CMD npm start