# llm-vid-stream

A pipeline for processing an RTSP stream through machine learning (computer vision) and passing the output through to an LLM for generation of additional information.

## First Attempt at Setting Up the Stream

Using the NVIDIA Jetson Xavier Developer Kit, we tried to run a Docker container using the NVIDIA jetpack-l4t Docker image and ```jetson-utils``` repo. We used the ```jetson-utils``` repo instead of the ```jetson-inference``` repo because the latter contains libraries that are not relevant for running the video stream. As a result, we had to install several dependencies in order for the Dockerfile to properly run. However, this proved to be a lengthy and repetitive process and ultimately did not work. Therefore, we decided to use the ```jetson-inference``` repo in order to not worry about any dependencies that may or may not have been installed. After ensuring that the entire system works, we will go back and focus on trimming down the Docker images.

Made by Nikhil and Rushil Gupta
