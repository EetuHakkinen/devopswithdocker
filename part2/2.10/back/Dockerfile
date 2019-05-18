FROM ubuntu:16.04

WORKDIR /
COPY / .
RUN apt-get update 
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install

ENV NODE_ENV production

CMD [ "npm", "start" ]