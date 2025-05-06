# 📰 Read Articles — Fullstack Flask Web App

**Read Articles** is a full-stack web application built with the Flask framework. It displays articles stored in a SQLite database and follows a clean, modular project structure. This project serves as a skill demonstration of backend setup, templating, and ORM integration with SQLAlchemy.

---

## 🛠️ Tech Stack

- **Backend**: Python, Flask
- **Database**: SQLite (via SQLAlchemy ORM)
- **Frontend**: HTML, CSS, Bootstrap
- **Tooling**: Virtualenv

---

## ⚙️ Local Setup
- Clone the project
- Run `setup.sh`

---

## ▶️ Local Development Run
- `local_run.sh` It will start the flask app in `development`. Suited for local development

---

## 📂 Folder Structure

- `db_directory` has the sqlite DB. It can be anywhere on the machine. Adjust the path in ``application/config.py`. Repo ships with one required for testing.
- `application` is where our application code is
- `.gitignore` - ignore file
- `setup.sh` set up the virtualenv inside a local `.env` folder. Uses `pyproject.toml` and `poetry` to setup the project
- `local_run.sh`  Used to run the flask application in development mode
- `static` - default `static` files folder. It serves at '/static' path. More about it is [here](https://flask.palletsprojects.com/en/2.0.x/tutorial/static/).
- `static/bootstrap` We have already added the bootstrap files so it can be used
- `static/style.css` Custom CSS. You can edit it. Its empty currently
- `templates` - Default flask templates folder


```
├── application
│   ├── config.py
│   ├── controllers.py
│   ├── database.py
│   ├── __init__.py
│   └── models.py
├── db_directory
│   └── test.db
├── local_run.sh
├── local_setup.sh
├── main.py
├── poetry.lock
├── pyproject.toml
├── readme.md
├── static
│   ├── bootstrap
│   │   ├── css
│   │   │   ├── bootstrap.css
│   │   │   ├── bootstrap.css.map
│   │   │   ├── bootstrap-grid.css
│   │   │   ├── bootstrap-grid.css.map
│   │   │   ├── bootstrap-grid.min.css
│   │   │   ├── bootstrap-grid.min.css.map
│   │   │   ├── bootstrap-grid.rtl.css
│   │   │   ├── bootstrap-grid.rtl.css.map
│   │   │   ├── bootstrap-grid.rtl.min.css
│   │   │   ├── bootstrap-grid.rtl.min.css.map
│   │   │   ├── bootstrap.min.css
│   │   │   ├── bootstrap.min.css.map
│   │   │   ├── bootstrap-reboot.css
│   │   │   ├── bootstrap-reboot.css.map
│   │   │   ├── bootstrap-reboot.min.css
│   │   │   ├── bootstrap-reboot.min.css.map
│   │   │   ├── bootstrap-reboot.rtl.css
│   │   │   ├── bootstrap-reboot.rtl.css.map
│   │   │   ├── bootstrap-reboot.rtl.min.css
│   │   │   ├── bootstrap-reboot.rtl.min.css.map
│   │   │   ├── bootstrap.rtl.css
│   │   │   ├── bootstrap.rtl.css.map
│   │   │   ├── bootstrap.rtl.min.css
│   │   │   ├── bootstrap.rtl.min.css.map
│   │   │   ├── bootstrap-utilities.css
│   │   │   ├── bootstrap-utilities.css.map
│   │   │   ├── bootstrap-utilities.min.css
│   │   │   ├── bootstrap-utilities.min.css.map
│   │   │   ├── bootstrap-utilities.rtl.css
│   │   │   ├── bootstrap-utilities.rtl.css.map
│   │   │   ├── bootstrap-utilities.rtl.min.css
│   │   │   └── bootstrap-utilities.rtl.min.css.map
│   │   └── js
│   │       ├── bootstrap.bundle.js
│   │       ├── bootstrap.bundle.js.map
│   │       ├── bootstrap.bundle.min.js
│   │       ├── bootstrap.bundle.min.js.map
│   │       ├── bootstrap.esm.js
│   │       ├── bootstrap.esm.js.map
│   │       ├── bootstrap.esm.min.js
│   │       ├── bootstrap.esm.min.js.map
│   │       ├── bootstrap.js
│   │       ├── bootstrap.js.map
│   │       ├── bootstrap.min.js
│   │       └── bootstrap.min.js.map
│   └── style.css
└── templates
    ├── articles_by_author.html
    └── articles.html
```
