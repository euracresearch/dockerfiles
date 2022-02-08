appname := alpine-httpd-php
version := 2.8.1

all: build

build:
	docker build -t eurac/$(appname):$(version) .

push:
	docker push eurac/$(appname):$(version)

clean:
	docker rmi -f eurac/$(appname):$(version)
