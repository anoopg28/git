FROM ubuntu:latest
LABEL "Creator"="Anoop"
LABEL "Project"="Demo"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update -y
RUN apt install git apache2 -y
EXPOSE 80
CMD ["/usr/sbin/apachectl","-D","FOREGROUND"]
WORKDIR /var/www/html
VOLUME /var/log/apache2
ADD anoop.tar.gz /var/www/html
