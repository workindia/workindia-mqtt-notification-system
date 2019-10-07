FROM ubuntu:latest
MAINTAINER Moiz Arsiwala <moiz.arsiwala@workindia.in>
ENV PYTHONUNBUFFERED 1
RUN apt-get -y update
RUN apt-get install -y mosquitto mosquitto-clients
RUN touch /etc/mosquitto/passwd
RUN mosquitto_passwd -b /etc/mosquitto/passwd test test
RUN mkdir /src;
WORKDIR /src
EXPOSE 1883 9001
