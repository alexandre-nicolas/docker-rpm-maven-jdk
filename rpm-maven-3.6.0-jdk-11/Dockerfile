FROM maven:3.6.0-jdk-11
MAINTAINER Alexandre Nicolas <a.nicolas@atolcd.com>

# Shutting down command line warnings
ENV DEBIAN_FRONTEND noninteractive

# Install dependancies
RUN apt-get update && \
  apt-get install -y --allow-unauthenticated apt-utils && \
  apt-get install -y --allow-unauthenticated rpm

# Cleaning
RUN apt-get clean
ENV DEBIAN_FRONTEND teletype
