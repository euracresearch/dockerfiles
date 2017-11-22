FROM alpine:latest
MAINTAINER Eurac SSN Group
RUN apk update
RUN apk add git --no-cache
ADD caddy /caddy 
ENTRYPOINT ["/caddy"]
