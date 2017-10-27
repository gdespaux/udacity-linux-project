# Overview
This project involved configuring a new Ubuntu instance on Amazon Lightsail. The Item Catalog project was then loaded and configured to be served using WSGI on Apache.

# Usage
IP Address: 18.220.145.79
SSH Port: 2200
Project URL: http://myudacityflaskapp.twilightparadox.com/

# Summary
After the bare install and update, the following notable packages were installed:
- Apache
- Postgres
- mod_wsgi

Apache was configured to use WSGI directed to `myapp.wsgi` in liue of an html page.

In Postgres, a `catalog` user and database were added to allow the Python app to connect.

Minor changes were made to the Item Catalog project to connect to a Postgres database instead of SQLite. Thanks to ssqlalchemy, this was a painless process.
