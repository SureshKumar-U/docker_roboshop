FROM node:20-slim
WORKDIR /opt/users
COPY package.json .
COPY *.js .
RUN npm install
ENV REDIS_URL="redis://redis:6379" \
    MONGO_URL="mongodb://mongo:27017/users"
ENTRYPOINT ["node"]
CMD ["server.js"]

