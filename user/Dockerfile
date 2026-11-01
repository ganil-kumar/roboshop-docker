FROM node:20
# this creates /app and move there
WORKDIR /app1
ENV MONGO="true" \
    REDIS_URL="redis://redis:6379" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
EXPOSE 8080
COPY package.json .
COPY *.js .
RUN npm install
CMD [ "node", "server.js" ]