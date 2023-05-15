FROM node:16 as Production

WORKDIR /usr/src/client

COPY package.json .
COPY package-lock.json .

RUN npm install

COPY . .

RUN npm run build

CMD [ "sh", "-c", "npm run start:production" ]