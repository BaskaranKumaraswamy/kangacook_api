# kangacook_api


First CommandLine
  -- -----------
1 python3 --version

2 python3 -m venv .venv

3 cd .\.venv\

4 cd .\Scripts\

5 .\activate

6 pip install django

7 pip install djangorestframework

8 django-admin startproject drinks .

9 python manage.py runserver

10 python manage.py runserver



Second CommandLine
  -- -----------
1 cd .\.venv\Scripts\

2 python manage.py migrate

3 python manage.py createsuperuser

4 python manage.py makemigrations drinks

5 python manage.py makemigrations drinks

6 python manage.py migrate


Url : http://127.0.0.1:8000/drinks/

Ref: https://www.youtube.com/watch?v=i5JykvxUk_A

seetings.py
==========


INSTALLED_APPS = [

'rest_framework',

'drinks',

'django.contrib.admin',

'django.contrib.auth',

'django.contrib.contenttypes',

'django.contrib.sessions',

'django.contrib.messages',

'django.contrib.staticfiles',

]

urls.py
========

from django.contrib import admin

from django.urls import path

from drinks import views

urlpatterns = [

path('admin/', admin.site.urls),

path('drinks/', views.drink_list),

]