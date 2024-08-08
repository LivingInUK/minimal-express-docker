# Minimalist Node.js Express Application in Docker

Initial code from https://nodejs.org/en/docs/guides/nodejs-docker-webapp/

## Build Docker image

To build manually:

    $ docker build -t entitymaker.com/pub/minimal-express:latest .
    $ docker login
    $ docker push entitymaker.com/pub/minimal-express:latest

## Running Docker image

    # run in foreground (ctrl-c to stop)
    $ docker run -p 44444:8080 -it entitymaker.com/pub/minimal-express

    # run in background as daemon
    $ docker run -p 44444:8080 -d entitymaker.com/pub/minimal-express
