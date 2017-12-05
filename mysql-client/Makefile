appname := mysql-client
version := 1.0

all: build

build:
	docker build -t eurac/$(appname):$(version) .

push:
	docker login 
	docker push eurac/$(appname):$(version)

clean:
	docker rmi -f eurac/$(appname):$(version)
