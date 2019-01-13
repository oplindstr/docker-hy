FROM ubuntu

EXPOSE 3000

RUN apt-get update
RUN apt-get install -y ruby
RUN apt-get install -y rails
RUN apt-get install -y tzdata
RUN apt-get install -y sudo
RUN sudo ln -fs /usr/share/zoneinfo/Europe/Helsinki /etc/localtime
RUN sudo dpkg-reconfigure -f noninteractive tzdata