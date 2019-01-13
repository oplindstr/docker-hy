FROM ubuntu

WORKDIR /front

EXPOSE 5000

COPY frontend-example-docker /front
RUN apt-get update
RUN apt-get install -y curl
RUN apt-get install -y gnupg
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y sudo
RUN sudo apt-get install -y nodejs
RUN npm install

ENTRYPOINT API_URL=http://localhost:8000 npm start