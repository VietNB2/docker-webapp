FROM ubuntu:16.04
LABEL author="VietNB2"

WORKDIR /root
COPY . .

RUN apt update -y
RUN apt install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install

CMD front_url=${front_url} npm start

