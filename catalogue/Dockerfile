FROM node:20 
WORKDIR /opt/server 
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO_URL=mongodb://mongodb:27017/catalogue \
    CATALOGUE_SERVER_PORT=8000 \
    GO_SLOW=5
ENTRYPOINT ["node"]
CMD ["server.js"]