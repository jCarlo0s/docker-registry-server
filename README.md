# Docker Registry Server

Hi, this is a  startup project for create a local registry for docker images
contains three main services:

1. Registry:2 This is the image of the registry provided by the docker team
2. Nginx just to implement https on the api but is not active for now
3. UI. we are using an existing project named docker-registry-frontend that have
   a minimalist interface to basic image management.

# How use the compose
First you need to clone this repo on the location do you want.

```bash
  git clone https://github.com/jCarlo0s/docker-registry-server.git
  cd docker-registry-server
```

Then just run:

```bash
  docker-compose up  
```
And thats all you need, if all works correctly you can make a curl request like:

```bash
  curl http://127.0.0.1:5000/v2/
```

And you will see an empty object:

```bash
  {}
```
