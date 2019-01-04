FROM ubuntu:16.04
WORKDIR /mydir
COPY  frontend-example-docker /mydir/
RUN apt-get update && apt-get install -y wget curl 
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash 
RUN apt install -y nodejs 
EXPOSE 5000
RUN npm install --save-dev webpack
CMD npm start 
