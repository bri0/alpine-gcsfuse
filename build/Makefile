default: build
build: docker
	mkdir -p dist
	rm -rf dist/*
	docker run -v `pwd`/dist:/dist brio/alpine-gcsfuse:go-1.9.1 cp /go/bin/gcsfuse /dist/gcsfuse

docker:
	docker build -t brio/alpine-gcsfuse:go-1.9.1 .
