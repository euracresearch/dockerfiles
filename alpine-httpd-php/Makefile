appname := alpine-httpd-php
version := 1.1

all: build

build:
	docker build -t eurac/$(appname):$(version) .

push:
	docker login 
	docker push eurac/$(appname):$(version)

clean:
	docker rmi -f eurac/$(appname):$(version)
