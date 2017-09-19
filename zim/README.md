# Zim - A Desktop Wiki in Docker

## Build

    docker build --build-arg HTTP_PROXY=proxy --build-arg HTTPS_PROXY=proxy -t memogarcia/zim .

## Run

    xhost local:root  ## in host machine
    docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=unix$DISPLAY memogarcia/zim
