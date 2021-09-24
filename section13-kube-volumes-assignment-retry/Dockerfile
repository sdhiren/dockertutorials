FROM node:14-alpine

WORKDIR /app

COPY package.json .

RUN npm install

COPY . /app

EXPOSE 3000

ENV STORY_FOLDER '/story'

CMD ["node", "app.js"]