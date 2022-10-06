# Backend
FROM ubuntu

LABEL maintainer="revocat"
ENV USERNAME=root
ENV PASSWORD=123456
ENV DB_HOST=localhost
ENV MYSQL_ROOT_PASSWORD=123456

RUN apt-get update
# RUN apt-get update
RUN apt install git -y
RUN apt install npm -y
RUN apt install nodejs -y


RUN mkdir /root/server
RUN mkdir /root/server/Conduit_NodeJS

# RUN git config --global http.sslverify false
# RUN git clone --recursive https://github.com/Varun-Hegde/Conduit_NodeJS.git
COPY Conduit_NodeJS /root/server/Conduit_NodeJS

WORKDIR /root/server/Conduit_NodeJS
RUN npm install
RUN npm start

