FROM node:20
WORKDIR /app
COPY package*.json .
RUN npm install
COPY service.js .
ENV MONGO_URL=mongodb://mongodb:27017/catalogue
    MONGO="true"
CMD ["node", "server.js"]
