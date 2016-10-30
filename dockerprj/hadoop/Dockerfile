FROM ubuntu:14.04
RUN useradd -ms /bin/bash osgdev
USER osgdev
RUN apt-get update
RUN apt-get install -y curl
RUN mkdir software
COPY requirements.txt /software/
