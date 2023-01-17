# Docker Hello World !!

Some compulsory file should exist:
1. Dockerfile -> contain all the command to build and run the docker container
2. .dockerignore -> to tell docker to ignore some file

### What is docker-compose ?
Automated docker deployment/build

### What is DOCKERFILE?
The blueprint of the docker. used to create docker image

```bash
# Install package
$ npm install

# Build the Dockerfile images
# docker build -t image-name /path/to/dockerfile
$ docker build -t mydocker .

# Run the docker
# docker run --name WhatNameYouGiveToContainer -p laptopport:dockerport -d Dockerimage
docker run --name thenameofmydocker -p 3000:3000 -d mydocker
```

### Dockerfile Command and explanation
| Command | What it do                                                     |
|---------|----------------------------------------------------------------|
| FROM    | The base image to be used                                      |
| RUN     | can run multiple command - can have multiple RUN in dockerfile |
| CMD     | can only run 1 command - can only have 1 CMD in dockerfile     |
| COPY    | copy file from-to                                              |
| EXPOSE  | expose docker port                                             |
| WORKDIR | working directory of the docker                                |