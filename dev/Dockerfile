FROM ubuntu:trusty
MAINTAINER Mattias Appelgren, mattias@ppelgren.se

WORKDIR /tmp

RUN apt-get update \
    && apt-get --yes --quiet upgrade \
    && apt-get --yes --quiet install git build-essential

# Set locale to use UTF-8
#RUN locale-gen en_US.UTF-8
#RUN update-locale LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
#ENV LANG en_US.UTF-8
#ENV LC_ALL en_US.UTF-8

