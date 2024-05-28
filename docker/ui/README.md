# Docker
## Conductor UI
This Dockerfile creates the conductor-ui image

## Building the image

Run the following commands from the project root.

`docker build -f docker/ui/Dockerfile-Ui -t conductor-ui:{tag} .`

## Running the conductor server

- use `WF_SERVER` to connect with specific conductor server (default http://localhost:8080)

`docker run -it -p 5000:5000 -e "WF_SERVER=http://conductor-server:8080" conductor-ui:{tag}`
