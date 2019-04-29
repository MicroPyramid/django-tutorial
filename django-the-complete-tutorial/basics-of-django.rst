Basics of Django
================

django-admin startproject <your project name>

django project comes with urls, settings, wsgi, templates (admin). You can extend it with apps.

django don't impose file structure and you have complete freedom on choosing the file/folder structure. Its better to keep modules in django apps with meaning ful names obviously.

settings
--------
This is where you store all settings related to the project like database type, autentication, template file path, static file path, session storage (either db or file storage), othe third party api keys, etc.

wsgi
----
This stands for Web Server Gateway Interface - That means it is the interface/entry-point between web server and your django project.

urls
----
This is where we map url to controller (python functions or classes)
