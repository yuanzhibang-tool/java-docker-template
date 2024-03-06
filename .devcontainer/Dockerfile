FROM openjdk:21-jdk-slim-bullseye
ARG DEBIAN_FRONTEND=noninteractive
RUN LC_ALL=C.UTF-8
RUN echo 'start build'

RUN sed -i 's/deb.debian.org/mirrors.ustc.edu.cn/g' /etc/apt/sources.list
RUN apt update --fix-missing
RUN apt install -y iputils-ping docker docker-compose nodejs maven curl protobuf-compiler

ENTRYPOINT tail -f /dev/null

