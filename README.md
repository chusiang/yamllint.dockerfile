# Docker image: yamllint

[![OS](https://img.shields.io/badge/os-alpine-blue.svg)](https://hub.docker.com/_/alpine/) [![Docker Hub](https://img.shields.io/badge/docker-yamllint-blue.svg)](https://hub.docker.com/r/chusiang/yamllint/) [![Download Size](https://images.microbadger.com/badges/image/chusiang/yamllint.svg)](https://microbadger.com/images/chusiang/yamllint "Get your own image badge on microbadger.com")

A Docker image for run the [yamllint][yamllint_github] on Alpine Linux.

[yamllint_github]: https://github.com/adrienverge/yamllint

## Supported tags and respective `Dockerfile` links

- `1.5`, `latest` [*(Dockerfile)*](https://github.com/chusiang/yamllint.dockerfile/blob/master/v1.5/Dockerfile)

## Build image

1. Get this project.

    ```
    $ git clone https://github.com/chusiang/yamllint.dockerfile.git
    ```

1. Go to workspace.

    ```
    $ cd yamllint.dockerfile/<REVERSION>
    ```

1. Bunild the image.

    ```
    $ docker build -t yamllint .
    $ docker build -t yamllint:<REVERSION> .
    ```

## Run container

1. Get image.

    ```
    $ docker pull chusiang/yamllint
    ```

1. Run the container.

    ```
    $ docker run --name yamllint -it chusiang/yamllint sh
    ```

1. Check container process.

    ```
    $ docker ps
    ```

1. Enter container with command line.

    ```
    $ docker exec -it yamllint bash
    ```

Enjoy it !

## History

### 2019

* 05/04: Add `1.5` image.

## License

MIT license from 2019.

## Author Information

1. [Chu-Siang Lai](https://github.com/chusiang/)
