FROM node:alpine

RUN mkdir -p /app

WORKDIR /app

COPY package.json .

COPY . /app

RUN npm install

RUN npm run prepare

EXPOSE 3000

CMD ["npm", "run", "dev"]
