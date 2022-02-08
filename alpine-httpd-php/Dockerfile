FROM alpine:latest

RUN apk update
RUN apk add apache2 php8-apache2 php8-tokenizer php8-mysqli php8-fileinfo php8-session php8-gd php8-curl php8-dom php8-zip php8-openssl php8-json php8-xmlreader --no-cache

RUN mkdir -p /run/apache2
RUN echo "ServerName localhost" >> /etc/apache2/httpd.conf

RUN rm -f /var/cache/apk/*

EXPOSE 80
ENTRYPOINT ["httpd", "-DFOREGROUND"]
