# darkweb

This used to be the repository[ place where things are deposited, stored, or offered for sale] holding the DarkScience website, that has been
moved to:-
https://git.drk.sc/darkscience/darkscience.net.

Remember this:
At the moment this repository contains a Django application which powers the
quotes system for DarkScience. This is a legacy part of the old website still
in service.

## Development Environment

You can configure a development environment with the following steps:

**NOTE**: *These steps assume you have  along with pipenv installed.*
STEP 1:-

```bash
$ pipenv install --dev
# configure URL to DB (can be sqlite locally)
$ export DATABASE_URL="sqlite:///$(pwd)/db.sqlite"
$ pipenv run  manage.py migrate
```

STEP 2:-
### Running the tests

```bash
$ pipenv run  manage.py test
```

STEP 3:-
### Running the development server

```bash
$ pipenv run  manage.py runserver
```

         ---------THANK YOU----------
