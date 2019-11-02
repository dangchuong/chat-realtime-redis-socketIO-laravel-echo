# Realtime chat app using Laravel, VueJS, Redis, Laravel Echo Server

## Installation:
- Clone this project

Run following command on root folder:

    - composer install
    - npm install
    - npm update
	- cp .env.example .env
	- laravel-echo-server init (then just select yes, but don't select HTTPS)

Open `resources/js/bootstrap.js` scroll to bottom and choose which host match to yours (production or development, probably you should choose `development`)

Then open your `.env` file and change database connection info as installed on your PC

Turn on Xampp, Access PHPMyadmin and create a database with the name you defined in `.env`

Setup Laravel Echo Server. Run: `laravel-echo-server init`. Just `yes` and choose `redis`

Open `laravel-echo-server.json` change `authHost` to your app's address

Run following command: 

	- php artisan migrate
	- php artisan serve
	- npm run watch (open in another terminal tab)
	- laravel-echo-server start
    - php artisan queue:work

Open browser in Chrome and another tab using incognito or other browser type (Safari, Firefox). Create an account and test your app

