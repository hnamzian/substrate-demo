__NOTE:__ This project is borrowed and enhanced from elkozman work:
  https://github.com/elkozmon/canvas-node-docker
# Canvas Node in Docker
Dockerfile for Parity's Canvas Node, a Substrate chain for smart contracts.

## Build Canvas docker image:

To build canvas docker image from Dockerfile:

`docker build . --tag canvas`

## Quick start

To run canvas node using docker command: 

```sh
docker run \
  -d -p 9944:9944 \
  --name canvas-node \
  --restart unless-stopped \
  canvas
```

## Run with docker-compose

For the first time you must build docker image from Dockerfile:

`docker-compose up -d`

From now on, you can run canvas node from prebuilt image by running:

`docker-compose up -d --no-build`

## Test your Node

Open the following URL from your browser and select __Local Node__:
https://paritytech.github.io/canvas-ui
