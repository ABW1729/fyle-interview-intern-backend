# Fyle Backend Challenge


### Install requirements

```
virtualenv env --python=python3.8
source env/bin/activate
pip install -r requirements.txt
```

### Reset DB

```
export FLASK_APP=core/server.py
rm core/store.sqlite3
flask db upgrade -d core/migrations/
```

### Start Server

```
bash run.sh
```

### Run Tests

```
pytest -vvv -s tests/

# for test coverage report
# pytest --cov
# open htmlcov/index.html
```

## Docker

### Build

```
docker-compose build
```

### Start Server

```
docker-compose up
```

### Run Tests

```
docker-compose run app pytest -vvv -s tests/
```


