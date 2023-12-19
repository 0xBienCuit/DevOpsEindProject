FROM node:17-alpine3.14
WORKDIR /backend
COPY package.json .
COPY index.js .
COPY . .
RUN npm install
EXPOSE 3000
CMD ["node", "index.js"]
