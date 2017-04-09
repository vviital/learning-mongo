FROM node

WORKDIR /opt/app
COPY package.json .
RUN npm install
COPY buildingQueryDocuments.js .
CMD node buildingQueryDocuments.js
