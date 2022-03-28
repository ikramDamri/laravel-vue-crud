## Backend deploy

-In the root folder, copy the .env.example to .env .
-In .env file you should find the DB name add the name to your MySQL DB

-Install required packages by running

```sh
composer install
```

Make sure composer and PHP are installed and configured on your machine (I used PHP8 for the developement environment)

-Run

```sh
php artisan key:generate
```

-Run

```sh
php artisan migrate:fresh --seed
```

Use the seed flag to add mock data into the database

-All those previous steps are only required to be ran on the first time, you dont need to re-run any of those later.

-Finally run

```sh
php artisan serve
```

to start the server locally
