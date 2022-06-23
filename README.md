# fastapi 

## requirements
* Python 3.10.4

### Setup
```bash
python -m venv venv
pip install fastapi
pip install "uvicorn[standard]"
uvicorn main:app --reload
```

### app project
```
.
├── app                        # "app" is a Python package
│         ├── __init__.py      # this file makes "app" a "Python package"
│         ├── main.py          # "main" module, e.g. import app.main
│         ├── dependencies.py  # "dependencies" module, e.g. import app.dependencies
│         └── routers          # "routers" is a "Python subpackage"
│         │   ├── __init__.py  # makes "routers" a "Python subpackage"
│         │   ├── items.py     # "items" submodule, e.g. import app.routers.items
│         │   └── users.py     # "users" submodule, e.g. import app.routers.users
│         └── internal         # "internal" is a "Python subpackage"
│             ├── __init__.py  # makes "internal" a "Python subpackage"
│             └── admin.py     # "admin" submodule, e.g. import app.internal.admin
```
