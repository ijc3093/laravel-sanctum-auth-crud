# Building and consuming using a restful api in laravel, php and mysql

# Instruction
- Step 1: Create Laravel Project
- Step 2: Add Database Details
- Step 3: Install Laravel Sanctum Pacakage
- Step 4: Setting Up Sanctum
- Step 5: Update Model and Run Migration
- Step 6: Build API Resources
- Step 7: Set Up Controllers
- Step 8: Create REST API Routes
- Step 09: Test REST API in Postman


- composer install (This is for creating new project)
- php artisan key:generate  (This is for creating new file)
- php artisan migrate (This is for connecting between database and php)
- php artisan serve (This is for running the project on terminal)

## Prerequisites
- PHP 7.1 or Higher
- Composer
- MySql
- Laravel 5.6 or Higher (laravel/framework": "5.7.*)
- Postman

# MYSQL

- Open terminal on your macbook and type command: PATH=$PATH:/usr/local/mysql/bin and press "enter"
- Then type command: mysql -u root -p and press "enter"
- If it asked for your password for root, you should type your password and press "enter"
- Make sure that your password for username should be match from MYSQL server
- type command: CREATE DATABASE `db_name`; and press "enter"
- type command: show databases; and press "enter"
- Make sure that database name called "db_name" should be existed in database system.
- leaving the mysql running......

# Execute db on LARAVEL
- type command: php artisan migrate

## API CRUD
- POST: http://localhost:8000/api/register
- POST: http://localhost:8000/api/login
- POST: http://localhost:8000/api/blogs
- GET: http://localhost:8000/api/blogs/{id}
- GET (ALL): http://localhost:8000/api/blogs
- PUT: http://localhost:8000/api/blogs/{id}
- DELETE: http://localhost:8000/api/blogs/{id}

# In api.php
- Route::post('login', [AuthController::class, 'signin']);
- Route::post('register', [AuthController::class, 'signup']);

## Modelo de resultado
