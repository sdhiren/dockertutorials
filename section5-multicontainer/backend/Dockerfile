FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

ENV MONGODB_USERNAME=dhiren
ENV MONGODB_PASSWORD=c3xs1bs

CMD ["npm", "start"]