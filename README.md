uv python install 3.12

uv init -p 3.12 --package

mkdir flask-microblog

uv sync

source .venv/bin/activate

which python

ls -l .venv/bin/python

system python von ubuntu ist bei /usr/bin/python

uv python ist unter deinem home directory

---
In src/app/app.py Flask instanzieren
```
from flask import Flask

app = Flask(__name__)

@app.route("/")
@app.route("/index")
def index():
    return "Hello, World!"
```

```
export FLASK_APP="app.app"
flask run
```
---

```
flask db init
flask db migrate -m "users table"
flask db upgrade
flask db migrate -m "posts table"
flask db upgrade
```

---