# Presta dockerized dev environment

* www contains all the source files
* db-data persists database

## Usage

### Start

```sh
git clone git@github.com:tswfi/presta-docker-dev.git
cd presta-docker-dev
docker-compose up
```

and open http://localhost/

### Reset

```sh
rm -rf db-data/* www/*
docker-compose up --force-recreate
```