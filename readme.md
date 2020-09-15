Steps for connecting django with mysql in windows


1)Got to settings.py file in the database section change dbsqlite3 to mysql.
by doing
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

2)Installing Mysqlclient for windows
a)Go to this <a href="https://www.lfd.uci.edu/~gohlke/pythonlibs/#mysqlclient">link</a>
b)Download this file "mysqlclient‑1.4.6‑cp37‑cp37m‑win32.whl"
c)Install it using
pip install mysqlclient‑1.4.6‑cp37‑cp37m‑win32.whl
4)Execute the command->python manage.py migrate
5)Exceute ->python manage.py runserver
