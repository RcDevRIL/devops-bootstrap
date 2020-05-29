FROM alpine:latest

RUN apk update
RUN apk add bash
RUN apk add apache2
COPY index.html ./www/
COPY default.conf /etc/apache2/sites-enabled
EXPOSE 8080
CMD httpd -D FOREGROUND