FROM ubuntu:16.04

WORKDIR /usr/local/
COPY / .
RUN apt-get update
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN npm install

EXPOSE 5000

ENV NODE_ENV production

CMD ["npm", "start"]