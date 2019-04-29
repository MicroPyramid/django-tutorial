django setup and configuration
==============================

We can start the installation to a minimum complex solution, we will add more complex setup configurations as we develop secure, high performance applications.

Basic thumb rules
=================
1. Use virtualenv always to isolate your projects python packages.
2. Never keep any sensitive information in settings. Use ENV variables instead.


I recommend to install the following in linux to get started.

sudo apt-get install python-dev, python-virutalenv, python-pip

now lets create directory of your choice and create virtualenv in it.

virtualenv env

then use the virtual env.

source env/bin/activate

install django with pip

pip install django

create django project

django-admin startproject <your-project-name>

run to see the django starting page

python manage.py runserver

now you can open the local development site at http://localhost:8000/