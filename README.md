# Build a REST API with Django Rest Framework and MySQL

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
## Installation
Install Environment
```sh
sudo apt install python3
sudo apt install python3-pip
```
Install the dependencies and devDependencies and start the server.

```sh
mkdir project
pip install virtualenv
virtualen env_djs
source env/bin/activate
```
Preparation project
```sh
git clone https://github.com/jumadilakbar/django-service.git
cd django-service
pip install -r requirement.txt
python manage.py showmigrations
python manage.py migrate
```
Run project
```sh
python manage.py runserver
```
## Endpoint
`POST : http://127.0.0.1:8000/todos/`  => Insert new data

`body:`
```json
{
    "text":"test data 1"
}
```

`GET : http://127.0.0.1:8000/todos/`  => GET all data todo

`output:`
```json
[
    {
        "id": 1,
        "text": "test data 1"
    },
    {
        "id": 3,
        "text": "test data 3"
    }
]
```

`PUT : http://127.0.0.1:8000/todos/$todo_id`  => Update data on todo

`body:`
```json
{
    "text":"test data baru"
}
```

`DELETE : http://127.0.0.1:8000/todos/$todo_id`  => Delete data on todo by id

`output:`
```json
{
    "message": "success delete"
}
```

##### Contact
`Email`: muhamadjumadilakbar@gmail.com

