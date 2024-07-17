# kangacook_api


First CommandLine
  -- -----------
1 python3 --version
2 python3 -m venv .venv
3 . .\.venv\bin\activate
4 cd .\.venv\
5 cd .\Scripts\
6 .\activate
7 pip install django
8 pip install djangorestframework
9 django-admin startproject drinks .
10 python manage.py runserver
11 python manage.py runserver


Second CommandLine
  -- -----------
1 cd .\.venv\Scripts\
2 python manage.py migrate
3 python manage.py createsuperuser
4 python manage.py makemigrations drinks
5 python manage.py makemigrations drinks
6 python manage.py migrate
