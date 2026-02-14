# Docker Static Website
## Description

This project demonstrates how to containerize a static website using Docker.  
The website is served using an Nginx container built from a custom Dockerfile.

It showcases basic Docker concepts including:
- Building images
- Running containers
- Port mapping
- Copying files into images

## Project Structure

.
├── Dockerfile
└── website/
    ├── index.html
    ├── css/
    └── src/

##How it works
The base image is nginx:alpine
All files from ./website directory are copied into Nginx's default web directory
Docker exposes port 80, mapped to host port 8080
Running the container server the static website into browser

##Build the docker image
docker build -t my-site .

## Run the Container

docker run -p 8080:80 my-site
Open in browser: http://localhost:8080

##What I learned
Basic Docker image creation
Copying files into containers
Exposing ports and mapping to host
Serving a multi-asset static website (HTML, CSS, JS) via Nginx

