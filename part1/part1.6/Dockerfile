FROM ubuntu:16.04
WORKDIR /mydir
COPY  backend-example-docker /mydir/ 
RUN apt-get update && apt-get install -y wget curl nano
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash 
RUN apt install -y nodejs 
EXPOSE 8000
RUN npm install --save-dev cross-env
VOLUME /mydir/
CMD FRONT_URL=<part1/part1.5/> npm start