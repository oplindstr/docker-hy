FROM ubuntu

WORKDIR /back

EXPOSE 8000

COPY backend-example-docker /back
RUN apt-get update
RUN apt-get install -y curl
RUN apt-get install -y gnupg
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y sudo
RUN sudo apt-get install -y nodejs
RUN npm install

ENTRYPOINT FRONT_URL=http://localhost:5000 npm start