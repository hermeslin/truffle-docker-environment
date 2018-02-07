FROM node:9.5
MAINTAINER hermeslin <mercury.iwork@gmail.com>

RUN apt-get clean && apt-get update && apt-get install -y locales
RUN echo "en_US.UTF-8 UTF-8" > /etc/locale.gen
RUN locale-gen
RUN export LC_ALL=en_US.UTF-8 && export LANG=en_US.UTF-8 && export LANGUAGE=en_US.UTF-8

RUN mkdir /Ethereum
WORKDIR /Ethereum

RUN npm install -g truffle