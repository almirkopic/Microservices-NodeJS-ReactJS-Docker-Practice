FROM node:alpine

WORKDIR /app
COPY package.jsonn ./
RUN npm install
COPY ./ ./

CMD ["npm", "start"]