FROM node:20-alpine

WORKDIR /app

# writing these 3 lines so that npm install can be cached
COPY ./package.json ./package.json
COPY ./package-lock.json ./package-lock.json
RUN npm install

COPY . . 


EXPOSE 3000

CMD ["node", "index.js"]
