# Simple docker-compose example

[![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-Ready--to--Code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/bitsnaps/hello-docker-compose)


This example uses docker-compose tool to spin up two containers (aka services):
- Flask rest api (providing a list of products in json format), image size: ~702Mb
- A simplest php web page to list json products, image size: 417Mb

## How to run:
```
docker-compose up
```
Then browse to `http://localhost:5000/` and you can change source and see the udpates live...

## How to stop:
Just run:
```
docker-compse down
```
Docker images will be cached in your system, check out:
```
docker images
```
## Known issue:
The total size is > 1Gb, this can be optimized if you use a smaller docker images (e.g. alpine...).
