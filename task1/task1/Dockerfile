FROM ubuntu:20.04

LABEL maintainer="Irina Chizh"

RUN apt update
RUN apt install -y -q nginx

COPY default /etc/nginx/sites-available/default

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 8080/tcp

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]


