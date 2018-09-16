FROM ubuntu:16.04
MAINTAINER lingaswamy
RUN apt-get update && \
    apt-get install -y curl 
RUN curl -sL https://deb.nodesource.com/setup_6.x -o /opt/nodesource_setup.sh
RUN bash /opt/nodesource_setup.sh
RUN apt-get install nodejs -y
RUN apt-get install build-essential -y
COPY hello.js /opt/hello.js
EXPOSE 8080
CMD ["/usr/bin/node", "/opt/hello.js"]



