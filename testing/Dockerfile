FROM node:latest

WORKDIR /app

# As many args as you want but the end will be the default of /app for our case
COPY package.json package-lock.json ./

RUN npm ci
COPY ./hello.js ./
ENV FORCE_COLOR=1

CMD ["node", "hello.js"]
