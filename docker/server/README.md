# Docker
## Conductor server
This Dockerfile creates the conductor-server image

## Building the image

Run the following commands from the project root.

`docker build -f docker/server/Dockerfile-Server -t conductor-server:{tag} .`

## Running the conductor server

- use `CONFIG_PROP` environment variable to use specific config file 

`docker run -it -p 8080:8080 -e "CONFIG_PROP=config-postgres-es7.properties" conductor-server:{tag}`