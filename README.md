##Laravel 4 - Starter Kit

This is a Laravel 4 Starter Kit, it will help you getting started with Laravel 4.

It includes examples on how to use the framework itselff and how to use some packages, like the awesome [Sentry 2](https://github.com/cartalyst/sentry) package.

-----

##Included goodies

* Twitter Bootstrap 2.3.0
* jQuery 1.9.1
* Custom CLI Installer
* Custom Error Pages:
	* 403 for forbidden page accesses
	* 404 for not found pages
	* 500 for internal server errors
* Cartalyst Sentry 2 for Authentication and Authorization
* Back-end
	* User and Group management
	* Manage blog posts and comments
* Front-end
	* User login, registration, forgot password
	* User account area
	* Simple Blog functionality
* Packages included:
	* [Cartalyst Sentry 2](https://github.com/cartalyst/sentry)
	* [Jason Lewis Expressive Date](https://github.com/jasonlewis/expressive-date)
	* [Opauth](https://github.com/opauth/opauth)

-----

##How to Install

###1) Downloading
####1.1) Clone the Repository

	git clone http://github.com/brunogaspar/laravel4-starter-kit your-folder

####1.2) Download the Repository

	https://github.com/brunogaspar/laravel4-starter-kit/archive/master.zip

-----

###2) Install the Dependencies via Composer
#####2.1) If you don't have composer installed globally

	cd your-folder
	curl -s http://getcomposer.org/installer | php
	php composer.phar install

#####2.2) For globally composer installations

	cd your-folder
	composer install

-----

###3) Setup Database

Now that you have the Laravel 4 cloned and all the dependencies installed, you need to create a database for it.

After the database is created, open the file `app/config/database.php` and update the needed entries, just like in Laravel 3.

-----

###5) Use custom CLI Installer Command

Now, you need to create yourself a user and finish the installation.

Use the following command to create your default user, user groups and run all the necessary migrations automatically.

	php artisan app:install

-----

###6) Opauth Configuration for user authentication via Facebook (or any other supported authentication providers by Opauth)
1. Create a Facebook application at https://developers.facebook.com/apps/
   - Remember to enter App Domains
   - "Website with Facebook Login" must be checked, but for "Site URL", you can enter any landing URL.
2. Open the file `app/config/opauth.php` and update it with at least `App ID` and `App Secret`.

-----

###6) Accessing the Administration

To access the administration page, you just need to access `http://your-host/public/admin` on your browser and it will automatically redirect you to the login page, in the login page, just fill in and submit the form.

After you being authenticated, you will be redirected back to the administration page.

-----

Have fun :)

###LICENSE

> Version 1, December 2009

> Copyright (C) 2009 Philip Sturgeon <email@philsturgeon.co.uk>

 Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long
 as the name is changed.

> DON'T BE A DICK PUBLIC LICENSE
> TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

 1. Do whatever you like with the original work, just don't be a dick.

     Being a dick includes - but is not limited to - the following instances:

	 1a. Outright copyright infringement - Don't just copy this and change the name.
	 1b. Selling the unmodified original with no work done what-so-ever, that's REALLY being a dick.
	 1c. Modifying the original work to contain hidden harmful content. That would make you a PROPER dick.

 2. If you become rich through modifications, related works/services, or supporting the original work,
 share the love. Only a dick would make loads off this work and not buy the original works
 creator(s) a pint.

 3. Code is provided with no warranty. Using somebody else's code and bitching when it goes wrong makes
 you a DONKEY dick. Fix the problem yourself. A non-dick would submit the fix back.

