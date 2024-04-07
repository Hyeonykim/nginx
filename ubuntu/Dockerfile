FROM ubuntu:22.04

RUN apt-get update
RUN apt-get install -y nginx keepalived vim

RUN adduser --disabled-password --gecos "" nginx

RUN mv /etc/nginx/nginx.conf /etc/nginx/nginx.conf.bak
RUN ln -s /etc/proxy/nginx.conf /etc/nginx/nginx.conf

CMD ["/bin/bash", "-c", "service nginx start;sleep 10000000000000000000"]
