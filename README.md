[Carceres](https://github.com/Delor4/Carceres)
===================
Parking Management System by SKS
---

Clone repository:
```
git clone https://github.com/Delor4/Carceres.git
cd Carceres
git submodule update --init --recursive
```

RESTful HTTP API using [Flask](https://github.com/pallets/flask), [Flask-Restful](https://github.com/flask-restful/flask-restful) and [SQLAlchemy](https://github.com/zzzeek/sqlalchemy)
-------------------
You need:

- [Python](https://www.python.org/) ver. min. 3.6
- [pip](https://pypi.org/project/pip/)
- (optional) [virtualenv](https://pypi.org/project/virtualenv/)

```
cd app
```

- Install requisite packages:
```shell
$ make install
```

- Create tables:
```shell
$ make init_db
```

- Run service:
```shell
$ make run
```

More info: [CarceresBE](https://github.com/Delor4/CarceresBE)

---

Frontend using [Vue.js](https://vuejs.org/) and [Bootstrap](https://getbootstrap.com/)
----

You need:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

```
$ cd carceres
```

- Install dependences:
```
$ npm install
```

- Run site:
```
$ make run
```

- (Optional) Build static files:
```shell
$ make build
```

More info: [CarceresFE](https://github.com/Delor4/CarceresFE)

---

Conteners by [Docker](https://www.docker.com/)
-----

- Make and run docker image
```shell
$ make all
```

To update database in docker image:

```shell
$ docker exec -it <image_name> /bin/bash`
```
and then
```shell
$ make init_db
```

More info: [CarceresC](https://github.com/Delor4/CarceresC)

---
