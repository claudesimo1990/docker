FROM nginx:latest

MAINTAINER Claude Simo <jeanclaude.simo@abus-kransysteme.de>

ARG crt
ARG key
ARG fastcgi
ARG nginx_conf
ARG default_conf

ADD $nginx_conf /etc/nginx/nginx.conf
ADD $default_conf /etc/nginx/conf.d/default.conf

ADD $fastcgi /etc/nginx/fastcgi.conf

COPY $crt /etc/nginx/config/localhost.crt
COPY $key /etc/nginx/config/localhost.key