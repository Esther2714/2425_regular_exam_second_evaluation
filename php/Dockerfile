FROM node:latest
ADD ./online-chess
WORKDIR /app
RUN npm install 
RUN npm audit fix || :
RUN npm audit fix 
EXPOSE 3000
CMD node server.js
