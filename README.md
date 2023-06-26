# mypythondjframeworksite (Polls App)

## Django CLI

### Run
```
$ python manage.py runserver
```
OR
```
$ python manage.py runserver 8080
```

### Project

Create
```
python3 manage.py startapp polls[app_name]
```

Check
```
python3 manage.py check
```

### Database

Initial migration of Django Apps located at ```project_dir/settings.py```.
```
python manage.py migrate
```

Update the migrations of your app
```
python manage.py makemigrations polls[app_name]
```

Verifying the SQL of your ran migration (```your_app/migrations/0001_initial.py```)
```
python manage.py sqlmigrate polls 0001
```

#### SQLite

To check the tables
```
.tables
```

## Django Admin

Create the super user
```
$ python manage.py createsuperuser
```

- willianbarbosa / devwdougherty@outlook.com

## Technical Workflows

Apps on a Project
1. Check your app class config name ```at app/apps.py```
2. Add your AppConfig Class at ```project/settings.py```

URLs and Paths
1. Add your urlpatterns under ```app/urls.py```
2. Add/Include your urlpatterns under ```project/urls.py```

Database Models
1. Create your model under ```app/models.py```
2. Run ```python manage.py makemigrations [your_app_name]``` to create migrations for those models
3. Run ```python manage.py migrate``` to apply those changes to the database

## Tutorial

https://docs.djangoproject.com/en/4.2/intro/tutorial01/
https://docs.djangoproject.com/en/4.2/intro/tutorial02/#playing-with-the-api

