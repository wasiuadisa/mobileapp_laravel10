# mobileapp_laravel10

This is an API for an application with the authentication implemented in Laravel Sanctum.

## Usage

Change the *.env.example* to *.env* and add your database info

For SQLite, add
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
```

Create a database matching your parameters in ".env" fe

```
# Run the webserver on port 8000
php artisan serve
```

## Routes

```
# Public

POST   /api/login
@body: email, password

POST   /api/register
@body: name, email, password, password_confirmation

# Protected

POST    /api/logout
```