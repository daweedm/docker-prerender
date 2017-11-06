FROM node:stretch

MAINTAINER DaweedM <m@daweed.be>
RUN apt update -y && apt upgrade -y
RUN apt-get install git -y

RUN mkdir /root/prerender-cache
WORKDIR /root
RUN git clone https://github.com/prerender/prerender.git

WORKDIR /root/prerender
RUN npm install && npm install prerender-file-cache

COPY server-2.js .

ENV CACHE_ROOT_DIR=/root/prerender-cache
EXPOSE 3000
ENTRYPOINT node server-2.js