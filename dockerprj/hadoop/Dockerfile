####docker build -t "hadoop" .

FROM ubuntu:14.04
RUN useradd -ms /bin/bash osgdev
USER osgdev
RUN apt-get update
RUN apt-get install -y curl
RUN mkdir software
COPY requirements.txt /software/
ADD http://foo.com/package.tar.bz2 /tmp/
RUN apt-get install libc6-i386
RUN tar -xjf /tmp/package.tar.bz2 \
  && make -C /tmp/package \
  && rm /tmp/package.tar.bz2
