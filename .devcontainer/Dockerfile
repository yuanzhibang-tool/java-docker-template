FROM openjdk:8u342-jdk
ARG DEBIAN_FRONTEND=noninteractive
RUN echo 'start build'
RUN LC_ALL=C.UTF-8
# speed up build in China
RUN sed -i 's/deb.debian.org/mirrors.ustc.edu.cn/g' /etc/apt/sources.list
RUN apt update && apt install git -y
ENTRYPOINT tail -f /dev/null