all: build run
build:
	docker build -t ml_vid:1.0.0 -f Dockerfile-ml .

run:
	docker run --runtime nvidia --network host -p 1234:1234 -p 2234:2234 ml_vid:1.0.0
