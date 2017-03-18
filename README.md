# Learning_Note-Django

[Note from Video Class](https://www.youtube.com/watch?v=zTNA0MtZwso)

### Basice Concept

1. In Django, a web application is a project.

  * Using Django to start a project 
  
   ```
    $ django-admin.py startproject projectname
 
    $ find myfristDweb
     myfristDweb
     myfristDweb/manage.py
     myfristDweb/myfristDweb
     myfristDweb/myfristDweb/__init__.py
     myfristDweb/myfristDweb/settings.py
     myfristDweb/myfristDweb/urls.py
     myfristDweb/myfristDweb/wsgi.py 
   ```
    
    
  * Files we are internested in:
    * settings.py - configraution for the project. 
      Saying which project is this, what database you are going to, who are the user who can use it, what all the confiruation deatails for your particular application 
    * manage.py - never edit it
    * urls.py - decide your url path. This is the first thing you will need to do.
 
  * Run Development server (not product run)
    ```
    python manage.py runserver  
    ```
    ---
2. A project is made of many applications. Django includes many build-in apps in django.contrib for authentication, serving static files, secruity.

  * Start an app by following comment, then Django will generate some files for you.
   ```
   $ python manager.py startapp myfirstDapp
   $ find myfirstDapp
   myfirstDapp
   myfirstDapp/__init__.py
   myfirstDapp/admin.py
   myfirstDapp/apps.py
   myfirstDapp/migrations
   myfirstDapp/migrations/__init__.py
   myfirstDapp/models.py
   myfirstDapp/tests.py
   myfirstDapp/views.py
   ```
  * For setting up the application in the project, you will need to go back to the setting.py, then add into in the INSTALLED_APPS.
   
   ```
   INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'myfirstDapp',
   ]
   ```
     ---
     3.Using URL. http://www.something.com/foo. In Django, what you need to do is tell Djando what part of code that you are going to do with this URL.
     
     
      
      
    
