FROM ubuntu:16.04

WORKDIR /mydir 
RUN apt-get update && apt-get install -y wget curl 

COPY part1.4.sh .

RUN chmod 755 part1.4.sh
CMD ./part1.4.sh