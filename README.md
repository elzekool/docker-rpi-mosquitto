# Mosquitto (MQTT broker) docker image for Raspberry Pi 

Based on the [resin/rpi-raspbian:jessie](https://hub.docker.com/r/resin/rpi-raspbian/) image this Mosquitto image provides a 
MQTT broker for the Raspberry PI, the default configuration includes a MQTT endpoint on port 1883 and a WebSocket endpoint on port 9001.

## Running the image
The easiest way to run this image is to use [Hypriot OS](https://blog.hypriot.com/downloads/), with this OS you know 
you have a recent Docker version and that it works good on a Raspberry PI.

The image itself can be run with Docker compose: `docker-compose up -d`, Mosquitto will then be available on port 1883/9001.

## Building the image
The most recent version of the image is available on [Docker Hub](https://hub.docker.com/r/elzekool/rpi-mosquitto/) and building
is not needed. If you still want to build the image you can do that with `docker-compose build`.
