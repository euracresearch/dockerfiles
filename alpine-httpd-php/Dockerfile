FROM alpine:latest

RUN apk update 
RUN apk add apache2 php5-apache2 php5-mysqli php5-gd php5-curl php5-dom php5-zip php5-mcrypt php5-openssl php5-json php5-xmlreader --no-cache  

RUN mkdir -p /run/apache2
RUN echo "ServerName localhost" >> /etc/apache2/httpd.conf 

RUN rm -f /var/cache/apk/*

EXPOSE 80
ENTRYPOINT ["httpd", "-DFOREGROUND"]
