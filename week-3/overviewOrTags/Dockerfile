FROM node

WORKDIR /opt/app
COPY package.json .
RUN npm install
COPY overviewOrTags.js .
CMD node overviewOrTags.js
