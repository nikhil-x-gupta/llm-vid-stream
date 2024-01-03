all: build run
build:
	docker build -t cam_rtsp:1.0.0 -f Dockerfile-cam .

run:
	docker run --runtime nvidia --network host --device=/dev/video0 -p 1234:1234 cam_rtsp:1.0.0

