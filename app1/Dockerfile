FROM ubuntu 
RUN apt-get update 
## for apt to be noninteractive
ENV DEBIAN_FRONTEND noninteractive
ENV DEBCONF_NONINTERACTIVE_SEEN true
RUN apt-get install apache2 -y 
RUN apt-get install apache2-utils -y 
RUN apt-get clean 
EXPOSE 80
ADD . /var/www/html/app1
CMD apachectl -D FOREGROUND  
