# Dockerized 2048 Game

Containerized version of the open-source 2048 game, served with Nginx, published to Docker Hub, and deployed on Railway.

Original game by Gabriele Cirulli: https://github.com/gabrielecirulli/2048 (MIT License)

## Live demo
YOUR-RAILWAY-URL

## Docker Hub
https://hub.docker.com/r/maheen5008/t48

## Run locally
docker pull maheen5008/t48:latest
docker run -d -p 8080:80 maheen5008/t48:latest
Then open http://localhost:8080

## Build from source
docker build -t t48 .
docker run -d -p 8080:80 t48

## What I did
- Wrote the Dockerfile (Nginx base image, static files copied to /usr/share/nginx/html)
- Built and tested the image locally
- Pushed the image to Docker Hub
- Deployed the container on Railway with a public URL
- Originally developed in a CentOS Stream 9 VM using Vagrant and VirtualBox (Cloud Computing coursework)
