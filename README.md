# Cinema API

API service for cinema management written on DRF

## Installing using GitHub

```shell
git clone https://github.com/arsenmakovei/cinema-api.git
cd cinema-api

python -m venv venv
source venv/bin/activate (on macOS)
venv\Scripts\activate (on Windows)
pip install -r requirements.txt

set POSTGRES_HOST=<your db host>
set POSTGRES_DB=<your db name>
set POSTGRES_USER=<your db user>
set POSTGRES_PASSWORD=<your db password>
set SECRET_KEY=<your django secret key>

or you can create .env and set there

python manage.py migrate
python manage.py runserver
```

## Run with Docker

Docker should be installed

```shell
docker-compose build
docker-compose up
```

## Getting Access

Docker should be installed

* Create user via /api/user/register/
* Get access token via /api/user/token/

## Features

* JWT authenticated
* Admin panel /admin/
* Documentation is located at /api/doc/swagger/
* Managing orders and tickets
* Creating movies with genres, actors and image
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movie sessions
