
	Some stuff to remmeber when setting up the tutorial site.

Use python3.2 on command line

python3.2 manage.py runserve

ttp://127.0.0.1:8000/  #for server

python3.2 manage.py syncdb


# to make your own app on same level as manage
python3.2 manage.py startapp polls

#create your model


python3.2 manage.py sql polls

mysql -u root -pqwerty
show databases;

python manage.py validate – Checks for any errors in the construction of your models.
python manage.py sqlcustom polls – Outputs any custom SQL statements (such as table modifications or constraints) that are defined for the application.
python manage.py sqlclear polls – Outputs the necessary DROP TABLE statements for this app, according to which tables already exist in your database (if any).
python manage.py sqlindexes polls – Outputs the CREATE INDEX statements for this app.
python manage.py sqlall polls – A combination of all the SQL from the sql, sqlcustom, and sqlindexes commands.

python3.2 manage.py shell # gives us a django shell to test in

__str__() on Python 3 to your models

# Django provides a rich database lookup API that's entirely driven by
# keyword arguments

to get admin working uncomment the lines in url.py and settings.py

superuser: development password :qwerty

add an admin.py to each app so that admin knows its there.

in admin.py, set list desplay.
useful admin settings:
ist_display

list_filter[]
search_fields
date_hierarchy


django location code:

 python3.2 -c "
import sys
sys.path = sys.path[1:]
import django
print(django.__path__)"


To override a template, just do the same thing you did with base_site.html
 – copy it from the default directory into your custom directory, and make changes.
 


