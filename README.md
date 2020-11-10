# PettersonTube main repo

## Prerequisites

Docker and docker-compose should be installed to run it locally

In case you have not done this yet, you must [configure docker with gcloud](https://cloud.google.com/sdk/gcloud/reference/auth/configure-docker):

```bash
gcloud auth configure-docker
```

## Clone repository

```bash
git clone --recurse-submodules git@github.com:vitaliy-kovalenko/pettersontube.git
```

## Update submodules

```bash
git submodule update --remote --recursive
```

## Startup local environment

```bash
$ docker-compose up
```

This command will build images and launch docker containers for API, Webapp and MongoDB.

API: http://localhost:3000 <br>
Webapp: http://localhost:3001 <br>
MongoDB explorer: http://localhost:8081
