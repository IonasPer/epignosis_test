<p align="center"><img src="https://www.epignosishq.com/wp-content/uploads/2018/01/epignosis-logo-retina-1.png"></p>

 Epignosis Test Application
============================


## The System EER Diagram

[EER Diagram]https://github.com/IonasPer/epignosis_test/blob/master/Epignosis%20Test%20EER.png

## About The Technologies

To make this test project I have used the following technologies (frameworks/3d-party solutions)

- Laravel 5.7 
- PHP 7.3
- MYSQL
- mailtrap.io

## Setting Up Laravel

The local environment used can be set either via the Homestead (more information here: https://laravel.com/docs/5.7/homestead)
or `$ php artisan serve` through cli and XAMPP server (Apache/SQL).

To install laravel simply follow the instructions:
-First laravel requires composer. Visit the following URL and download composer to install it on your system.
https://getcomposer.org/download/
- Check composer is installed by typing `$ composer`
- You can clone or download this repository into your local machine.
- In the new directory type the following command to install all packages. 
    `$ composer install`
- Type `$ php artisan serve`, in the command line to  start serving at localhost.
-Create a Database. The database name will be used in the .env file.



## Mailtrap

A Mailtrap account is needed to utilize the mail notifications from a local environment. You can create an account or use your github account to signin in this link : [mailtrap]https://mailtrap.io/

In the Demo inbox at the top center of the page there is the Credentials Section. Add the username and password below in your local .env file.


## .env


In the .env file in the Laravel Project root make the following changes
```
DB_DATABASE="Your_database_name"
DB_USERNAME=root
DB_PASSWORD=

MAIL_DRIVER=smtp
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME="Your_mailtrap_username"
MAIL_PASSWORD="Your_mailtrap_password"
MAIL_ENCRYPTION=null
```

## Generate Encryption Key

Use `$ php artisan key:generate` to generate a key for laravel.

## Migrations and seeding

Once the .env is setup run with php artisan the migrations and seeders to create sample users. 
`$ php artisan migrate`

and once migrations are set 

`$ php artisan db:seed`

Note: the demo user credentials can be found in the users seeder

