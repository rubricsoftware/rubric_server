# DOCKER-VERSION 1.0.1
FROM ubuntu:14.04

# Update APT
RUN apt-get update

# Install Node.js and Node Package Manager (npm)
RUN apt-get -y install nodejs npm

# Bundle app source
COPY . /src

# Install app dependencies
RUN cd /src; npm install

EXPOSE  8080

CMD ["nodejs", "/src/index.js"]
