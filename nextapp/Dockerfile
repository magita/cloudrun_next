FROM node:current-slim

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000
#EXPOSE 8080
ENV PORT 3000

#ENV HOSTNAME "0.0.0.0"

CMD ["npm", "run", "start"]
