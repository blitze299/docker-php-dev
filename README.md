# Basic Docker Web Dev Box

Basic docker box for testing and developing reversy.
NOT FOR PRODUCTION USE!

##  Requirements

- This repo assumes you store your projects in  `~/code`.
- [Docker](https://docs.docker.com/engine/installation/) installed
- [Docker Compose](https://docs.docker.com/compose/install/) installed
- Databases must be imported seperately 

## Services

- PHP-FPM 7.1
- MySQL 5.7
- NGINX 1.10

## Accessing services

We're exposing NGINX and MySQL their ports, so you can just go to `http://127.0.0.1/` or `http://localhost/` from your browser and connect to MySQL from your client (eg: [Sequel Pro](https://www.sequelpro.com/)) using `127.0.0.1:3306` or `localhost:3306`.

To access MySQL from within your web applications you'll need to use `mysql` or `172.19.0.1` as host.

### Default MySQL credentials:

- **Username**: `docker`
- **Password**: `docker`
- **Database**: `docker`

## Installation / run

```bash
docker-compose up
```
