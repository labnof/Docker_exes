FROM ubuntu:16.04
WORKDIR /mydir
COPY  frontend-example-docker backend-example-docker /mydir/ 
RUN apt-get update && apt-get install -y wget curl nano
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash 
RUN apt install -y nodejs 
EXPOSE 8000 5000
RUN npm install --save-dev webpack  --save-dev cross-env
CMD npm start 