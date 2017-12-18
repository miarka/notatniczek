# Windows installation

## Scoop

Install PowerShell >= 3.0 . Then follow instructions from the link:

    https://www.outcoldman.com/en/archive/2014/07/20/scoop/

To avoid issues with JS on Windows remember to install nodejs:

    scoop install nodejs

## Database

    scoop install postgresql

### DB initialization

    pg_ctl init -D "D:\Projekty\postgresql\bazadanych.postgresql" -o "-E=UTF8"

### DB server start

    pg_ctl -D D:/Projekty/postgresql/bazadanych.postgresql -l D:/Projekty/postgresql/bazadanych.postgresql.log start

### DB server stop

    pg_ctl -D D:/Projekty/postgresql/bazadanych.postgresql stop

## Management

### Association with heroku remote for CLI

    heroku git:remote -a notatniczek

### Local run

    heroku local
