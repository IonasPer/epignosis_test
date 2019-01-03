<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## About The Technologies

To make this test project I have used the following technologies (frameworks/3d-party solutions)

- Laravel 5.7, PHP 7.3 used
- Maria_DB
- mailtrap.io

## Setting Up Laravel

The local environment used can be set either via the Homestead (more information here: https://laravel.com/docs/5.7/homestead)
or $ php artisan serve through cli and XAMPP server (Apache/SQL).

To install laravel simply follow the instructions:
-First laravel requires composer. Visit the following URL and download composer to install it on your system.
https://getcomposer.org/download/
- Check composer is installed by typing $ composer
- Create a new directory and type the following command there to install Laravel. 
    composer create-project --prefer-dist laravel/laravel epignosis_test
- Type $ php artisan serve and in the command line it should start serving at localhost.
- Now you can clone or download this repository into your local project.

## Mailtrap

A Mailtrap account is needed to utilize the mail notifications from a local environment. You can create an account or use your github account to signin in this link : https://mailtrap.io/

In the Demo inbox at the top center of the page there is the Credentials Section. Add the username and password below in your local .env file.

## .env

Before editing the .env create a Database, the database name will be used in the .env file.

In the .env file in the Laravel Project root make the following changes
DB_DATABASE="Your_database_name"    /* I use epignosis_dev*/
DB_USERNAME=root
DB_PASSWORD=

MAIL_DRIVER=smtp
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME="Your_mailtrap_username"
MAIL_PASSWORD="Your_mailtrap_password"
MAIL_ENCRYPTION=null



- [Simple, fast routing engine](https://laravel.com/docs/routing).

