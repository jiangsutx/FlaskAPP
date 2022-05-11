# FlaskAPP
This is the re-implemented code following The [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world), which is very useful for beginners of flask, datebases or web developers.

## Prerequisites
- `flask` for Python HTTP server 
- `flask_wtf` for flask forms
- `flask_sqlalchemy` for SQL and databases
- `flask_migrate` for database upgrade

## Structure

## Run
Start `flask` server:
```shell
export FLASK_APP=./microblog.py
flask run
```

Update database structure:
```shell
export FLASK_APP=./microblog.py
flask db migrate
flask db upgrade
```