FROM debian:latest

ENV NODE_VERSION 8.9.4

RUN mkdir /nodejs && \
    apt-get update -y && \
    apt-get install -y curl git xz-utils && \
    curl https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.xz | tar -xJf - -C /nodejs --strip-components=1

ENV PATH $PATH:/nodejs/bin
