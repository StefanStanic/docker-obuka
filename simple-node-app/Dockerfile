#This is our base image, found at docker hub
FROM node:14

#We move to a working directory in this case /usr/src/app
COPY package*.json ./

#install dependencies
RUN npm install

#move all code from our pc to this folder (usr/src/app)
COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]