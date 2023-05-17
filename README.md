# Laravel Chirper

## Introduction

This Laravel Chirper Full Stack App was developed based on Laravel Bootcamp, and it is based on Inertia (as a bridge between backend and frontend) and React.js.

## Before starting

Before starting development server, the following actions must be executed in the working directory:

### 1. Install dependencies

```bash
# install php dependency
composer install 

# install vite dependency
npm install
```

### 2. Create a personal copy of `env`

```bash
cp .env.example .env
```

### 3. Generate Laravel App Key

```bash
php artisan key:generate
```

### 4. Connect to MySQL Database (Modify Environment Variable)

Please make sure you have access to the database.

```text
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_db_name
DB_USERNAME=your_db_user_name
DB_PASSWORD=
```

To quickly set up a MySQL database on Docker

```bash
# pull image 
docker pull mysql

# start a container
docker run --name <my_mysql_instance_name> -e MYSQL_ROOT_PASSWORD=<root_password> -p 3306:3306 -d mysql
```

### 5. Populate a MySQL Database (Database Migration)

```bash
php artisan migrate
```



## Sanity check

To check the routes available, please run:

```bash
php artisan route:list
```

## To run the app

Run the development server:

```bash
php artisan serve
```

Run the Hot Module Replacement powered by Vite development server

```bash
npm run dev
```

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
