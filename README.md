# Docker image: yamllint

[![OS](https://img.shields.io/badge/os-alpine-blue.svg)](https://hub.docker.com/_/alpine/)
[![Docker Hub](https://img.shields.io/badge/docker-yamllint-blue.svg)](https://hub.docker.com/r/chusiang/yamllint/)

A Docker image for run the [yamllint][yamllint_github] on Alpine Linux.

[yamllint_github]: https://github.com/adrienverge/yamllint

## Supported tags and respective `Dockerfile` links

- `1.37`, `latest` [_(Dockerfile)_](https://github.com/chusiang/yamllint.dockerfile/blob/main/v1.37/Dockerfile)
- `1.15`, [_(Dockerfile)_](https://github.com/chusiang/yamllint.dockerfile/blob/main/v1.15/Dockerfile)

## Build image

1. Get this project.

   ```shell
   git clone https://github.com/chusiang/yamllint.dockerfile.git
   ```

1. Go to workspace.

   ```shell
   cd yamllint.dockerfile/<REVERSION>
   ```

1. Bunild the image.

   ```shell
   docker build -t yamllint .
   docker build -t yamllint:<REVERSION> .
   ```

## Run container

1. Get image.

   ```shell
   docker pull chusiang/yamllint
   ```

1. Run the container.

   ```shell
   docker run --name yamllint -it chusiang/yamllint sh
   ```

1. Check container process.

   ```shell
   docker ps
   ```

1. Enter container with command line.

   ```shell
   docker exec -it yamllint sh
   ```

Enjoy it !

## History

2025:

- 05/19: Add `1.37` image.

2019:

- 05/04: Add `1.15` image.

## License

MIT license from 2019.

## Author Information

1. [Chu-Siang Lai](https://github.com/chusiang/)
