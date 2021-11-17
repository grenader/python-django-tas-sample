# Hello world with Django deployed to TAS

https://github.com/grenader/python-django-tas-sample
## Requirements

```bash
Django 3.x
Python 3.x
```

# Initial set up for Mac

## Install pip
```
sudo python -m ensurepip —upgrade
```
look here: https://pip.pypa.io/en/stable/installation/

## Check that Pip is there
```
python -m pip —version
```

##We needed Python version 3. Install version 3.
```
brew install python3
```

## Install Django
```
python3 -m pip install Django
```

# Run the project

```bash
python manage.py migrate
```

```bash
python manage.py runserver
```

# Tanzu Application Service

## Deploy to TAS/PCF
```
cf login ...
cf push <your-app-name> -b https://github.com/cloudfoundry/python-buildpack.git
```
no manifest file needed.

## Check the application logs:
```
cf logs <your-app-name> --recent
```

# Oracle Driver
## Installed Oracle driver:
```
python3 -m pip install cx_Oracle
```
It’s also mentioned here: https://www.oracle.com/database/technologies/appdev/python/quickstartpythononprem.html#linux-tab

The driver will be along the libraries installed:
> Successfully installed Django-2.0 cx-Oracle-8.3.0 gunicorn-20.1.0 pytz-2021.3 setuptools-59.1.1

## Credit

The repository is gotten from [hacktivist123](https://github.com/hacktivist123/python-django-cloudfoundry-demo).
This Repository was inspired by [Argenis Osorio](https://github.com/argenisosorio/django-2-hello-world)'s Repository on [github](https://github.com/argenisosorio/django-2-hello-world)
# python-django-tas-sample
# python-django-tas-sample
