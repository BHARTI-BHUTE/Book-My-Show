FROM node:18

WORKDIR /app

COPY package.json package-lock.json ./

RUN npm install --legacy-peer-deps && npm install chokidar@3.5.3 --legacy-peer-deps

COPY . .

EXPOSE 3000

ENV NODE_OPTIONS=--openssl-legacy-provider
ENV PORT=3000

CMD ["npm", "start"]
