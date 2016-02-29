FROM debian:8

MAINTAINER debianrpxc@orangestems.co.uk

RUN apt-get update && apt-get install -y curl
RUN curl http://emdebian.org/tools/debian/emdebian-toolchain-archive.key | apt-key add -
RUN echo 'deb http://emdebian.org/tools/debian/ jessie main' > /etc/apt/sources.list.d/crosstools.list
RUN dpkg --add-architecture armhf
RUN apt-get update
RUN apt-get install -y crossbuild-essential-armhf gcc-arm-linux-gnueabihf

