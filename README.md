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

Grab a coffee while installer runs and open http://localhost/

Admin interface can be found in http://localhost/admin-dev/ (dev@vilkas.fi/admin)

Whole prestashop can be found in "www" folder.

### Reset

```sh
rm -rf db-data/* www/*
docker-compose up --force-recreate
```
