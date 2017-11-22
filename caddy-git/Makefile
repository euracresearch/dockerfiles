appname := caddy-git
version := 0.10.10

all: build

build:
	docker build -t eurac/$(appname):$(version) .

push:
	docker login 
	docker push eurac/$(appname):$(version)

clean:
	docker rmi -f eurac/$(appname):$(version)
