# FlaskAPP
This is the re-implemented code following The [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world), which is very useful for beginners of flask, datebases or web developers.

## Prerequisites
- `flask` for Python HTTP server 
- `flask_wtf` for flask forms
- `flask_sqlalchemy` for SQL and databases
- `flask_migrate` for database upgrade

## Structure

## Run
#### 1. Start `flask` server:
```shell
export FLASK_APP=./microblog.py
flask run
```

#### 2. Update database structure:
```shell
export FLASK_APP=./microblog.py
flask db migrate
flask db upgrade
```

#### 3. Use temporary debug email server:
```shell
python -m smtpd -n -c DebuggingServer localhost:8025
```
Then set up temporary server and start `flask`
```shell
export MAIL_SERVER=localhost
export MAIL_PORT=8025
export FLASK_APP=./microblog.py
flask run
```

#### 4. Run unit test:
```shell
python tests.py
```