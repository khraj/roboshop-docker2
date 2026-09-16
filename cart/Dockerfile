FROM node:20
WORKDIR /opt/server
COPY package.json .
EXPOSE 8080
COPY *.js .
RUN npm install
ENV CATALOGUE_PORT="8080" \
    CATALOGUE_HOST="catalogue" \
    REDIS_HOST="redis"
CMD ["nodejs", "server.js"]

