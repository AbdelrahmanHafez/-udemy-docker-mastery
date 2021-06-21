FROM node:12-alpine

EXPOSE 3000

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY ./ ./
RUN npm i && npm i -g pm2 && npm cache clean --force
CMD ["pm2-runtime", "./bin/www"]