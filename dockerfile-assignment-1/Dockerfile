FROM node:12-alpine

EXPOSE 3000:3000

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY ./ ./
RUN npm cache clean --force
RUN npm i
RUN npm i -g pm2
CMD ["pm2-runtime", "/usr/src/app/bin/www"]