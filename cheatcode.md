creating venv

py -m venv ./venv

activate the venv file 

py 
    source ./venv/bin/activate (MAC)
    source ./venv/scripts/activate (WINDOWS)


deactivate the venv file 

deactivate


creating a django project 

py 
    django-admin startproject (NAME //// optional) (LOCATION //// . for current)


checking all the libraries or packages that are intalled in this venv

py
 pip freeze


creating a django application 

py 
  django-admin startapp (APPNAME)


if you're having an error when you run django for the first time 

py 
pip install django


runserver 

py 
 py manage.py runserver

we are going to use 

from django.shortcuts import render (only when we have 'jinja' template, otherwise use HttpResponse to return raw html)
from django.http import HttpResponse

py 
from django.shortcuts import render
from django.http import HttpResponse


def index(request):
    html = "<h1>Hello World</h1>"
    return HttpResponse(html)




py manage.py makemigrations
py manage.py migrate


(psql)
Creating Database
CREATE SERVER (Name) OWNER (OwnerName/Username);

Seeing the list
\l