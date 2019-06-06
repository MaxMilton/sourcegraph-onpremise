# Sourcegraph On-Premise

## Setup

### Install

1. `docker volume create --name=sourcegraph-data` - Create our local data Docker volume manually, as it's declared as external to be more durable.
1. `docker-compose up -d`
1. Access your instance at `localhost:7080`!

### Upgrade

1. Edit `docker-compose.yml` (e.g. to update docker image tag)
1. `docker-compose pull; docker-compose up -d --build`
