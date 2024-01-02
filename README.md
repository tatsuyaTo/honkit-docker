honkit docker
====================================
[![Docker](https://github.com/workingted/honkit-docker/actions/workflows/docker-image.yml/badge.svg)](https://github.com/workingted/honkit-docker/actions/workflows/docker-image.yml)

## Build docker image

```
# cd docker
# docker build .
```

## Run honkit

```
# docker run --rm -d -p 4000:4000 -v `pwd`/sample:/work -w /work docker.io/tottidocker/honkit:latest honkit serve
```

