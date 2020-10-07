[Carceres](https://github.com/Delor4/Carceres)
===================
Parking Management System by SKS
---

RESTful HTTP API using [Flask](https://github.com/pallets/flask), [Flask-Restful](https://github.com/flask-restful/flask-restful) and [SQLAlchemy](https://github.com/zzzeek/sqlalchemy)
-------------------

```
cd app
```

- Install requisite packages:
```shell
$ pip install -r requirements.txt
```

- Create tables:
```shell
$ make init_db
```

- Run service:
```shell
$ python app.py
```
- List of endpoints:
- `/api/users`
    (Methods: `GET` `POST` `GET /<id>` `PUT /<id>` `DELETE /<id>`)

Don't forget add "Content-Type: application/json" header to your request!

Frontend using [Vue.js](https://vuejs.org/) and [Bootstrap](https://getbootstrap.com/)
---

```
$ cd carceres
```

- Install dependences:
```
$ npm install
```

- Run site:
```
$ npm run serve
```

- Build static files:
```shell
$ npm run build
```

Conteners by [Docker](https://www.docker.com/)
-----

- Make and run docker image
```shell
# make all
```

To update database in docker image:

```shell
# docker exec -it <image_name> /bin/bash`
```
and then
```shell
$ python create_db.py
```
