FROM ubuntu:14.04

MAINTAINER debianrpxc@orangestems.co.uk

RUN apt-get update && apt-get install -y curl
#RUN curl http://emdebian.org/tools/debian/emdebian-toolchain-archive.key | apt-key add -
#RUN echo 'deb [arch=armhf] http://ports.ubuntu.com trusty main' > /etc/apt/sources.list.d/ports.crosstools.list
RUN echo 'deb [arch=amd64,i386] http://archive.ubuntu.com/ubuntu trusty main universe multiverse' > /etc/apt/sources.list.d/deb-x86.list
RUN echo 'deb [arch=amd64,i386] http://archive.ubuntu.com/ubuntu trusty-updates main universe' >> /etc/apt/sources.list.d/deb-x86.list
RUN echo 'deb-src http://archive.ubuntu.com/ubuntu trusty main' > /etc/apt/sources.list.d/src.list
RUN echo '' > /etc/apt/sources.list
RUN dpkg --add-architecture armhf
RUN apt-get update
RUN apt-get install -y gcc-arm-linux-gnueabihf

