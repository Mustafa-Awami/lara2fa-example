# Lara2fa example application

This is an example use of [mustafa-awami/lara2fa](https://github.com/mustafa-awami/lara2fa) package.

## Installation

In order to test the application, you need to:

* Clone this repository

* Install packages and configuration:

    ```sh
    composer install
    npm install
    npm run build
    cp .env.example .env
    php artisan key:generate
    ```

* Migrate database.

    ```sh
    php artisan migrate
    ```

* Run a webserver
  * you can use the standard serve comand

    ```sh
    php artisan serve
    ```

  * or you can use a tool like [Laravel Herd](https://herd.laravel.com/) to serve your application over HTTPS, since features such as Passkeys require a secure connection, just make sure to change `APP_URL` in the `.env` file from `http://localhost` to somthing like `http://lara2fa-example.test`
