# docker-compose-bind9

### bind9 on docker compose with minimal changes

This is an docker compose based on [ubuntu/bind9](https://hub.docker.com/r/ubuntu/bind9) image
with named.conf and [example.com](zones/example.com.db) zone as example

### Installation

* Make sure you have already installed [docker](https://docs.docker.com/get-docker/) and [docker-compose](https://github.com/docker/compose)

* Clone the repo:
```console
$ git clone https://github.com/rbm0407/docker-compose-bind9
```

* Run docker-compose
```console
$ docker-compose up

```

* You can test if example.com is working with a dig request
```console
$ dig example.com @127.0.0.1
```

### Configuration

#### How to add a zone

* Create the zone file on zones directory
* Add on the named.conf
* Restart the container with `docker-compose restart`

### License

#### This repo with docker-compose file and examples:

* [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)

#### Third party licenses:

* [bind9](https://github.com/isc-projects/bind9/blob/main/LICENSE)
* [ubuntu](https://ubuntu.com/legal/intellectual-property-policy)

