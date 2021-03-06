# Dockerize simple NodeJS app with Vagrant configuration
![SFW](http://forthebadge.com/images/badges/kinda-sfw.svg)

Vagrant comes with support out of the box for using Docker as a provider. This allows for your development environments to be backed by Docker containers rather than virtual machines providing a good workflow for developing Dockerfiles.

## Prerequisites
* Mac OSX

Before you being, ensure you have the following in your system as well.
* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Docker for Mac](https://docs.docker.com/engine/installation/mac/#/docker-for-mac)

## Installaion
To run the project:
```bash
$ git clone <repo>
$ cd docker_nodejs_app
$ vagrant up
```

Go to `http://localhost:8080` to see the output

### To create Docker image
You will need to create docker hub account before you can do this.
```bash
$ cd docker_nodejs_app
$ docker build -t your-docker-hub-username/repo-name:tag-id .
```

### To run Docker image locally
```bash
$ docker run -p your-docker-hub-username/repo-name:tag-id
```
