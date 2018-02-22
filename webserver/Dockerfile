FROM docker.io/alpine:3.7
RUN mkdir -p /run/nginx
RUN apk update && apk add nginx
COPY default.conf /etc/nginx/conf.d/default.conf
COPY index.html /var/www
