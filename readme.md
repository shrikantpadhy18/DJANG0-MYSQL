Steps for connecting django with mysql in windows
<br>

1)Got to settings.py file in the database section change dbsqlite3 to mysql.
by doing
<br>

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'DATABASENAME',
        'USER': 'USERNAME',
        'PASSWORD': 'PASSWORD',
        'HOST': 'localhost',
        'PORT': 'PORT NO OF MYSQL'
    }
}
<br>

2)Installing Mysqlclient for windows
<br>
a)Go to this <a href="https://www.lfd.uci.edu/~gohlke/pythonlibs/#mysqlclient">link</a>
<br>b)Download this file "mysqlclient‑1.4.6‑cp37‑cp37m‑win32.whl"
<br>c)Install it using
pip install mysqlclient‑1.4.6‑cp37‑cp37m‑win32.whl
<br>4)Execute the command->python manage.py migrate
<br>5)Exceute ->python manage.py runserver
