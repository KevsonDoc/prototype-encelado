FROM node:alpine

WORKDIR /usr/app

COPY package*.json ./

RUN yarn

COPY . .

EXPOSE 3000

ENV CHOKIDAR_USEPOLLING=true
ENV CHOKIDAR_INTERVAL=500

CMD ["yarn" "dev"]
