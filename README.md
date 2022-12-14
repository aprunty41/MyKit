
## Introduction

[MyKit](https://devdojo.com/wave) is a Software as a Service Product for social media marketing tools that can help you build your social media presence. MyKit is built with [Wave](https://wave.com), [Laravel](https://laravel.com), [Voyager](https://voyager.devdojo.com), [TailwindCSS](https://tailwindcss.com),[Tallstack](https://tallstack.dev), and a few other awesome technologies. Here are some of the awesome features ✨:

 - [Authentication](https://wave.devdojo.com/docs/features/authentication)
 - [User Profiles](https://wave.devdojo.com/docs/features/user-profiles)
 - [User Impersonation](https://wave.devdojo.com/docs/features/user-impersonation)
 - [Subscriptions](https://wave.devdojo.com/docs/features/billing)
 - [Subscription Plans](https://wave.devdojo.com/docs/features/subscription-plans)
 - [User Roles](https://wave.devdojo.com/docs/features/user-roles)
 - [Notifications](https://wave.devdojo.com/docs/features/notifications)
 - [Announcements](https://wave.devdojo.com/docs/features/announcements)
 - [Fully Functional Blog](https://wave.devdojo.com/docs/features/blog)
 - [Out of the Box API](https://wave.devdojo.com/docs/features/api)
 - [Voyager Admin](https://wave.devdojo.com/docs/features/admin)
 - [Customizable Themes](https://wave.devdojo.com/docs/features/themes)


## Demo
View a live [demo here](https://wave.devdojo.com), or deploy your own instance to DigitalOcean, by clicking the button below.

<a href="https://cloud.digitalocean.com/apps/new?repo=https://github.com/thedevdojo/wave/tree/main" target="_blank"><img src="https://www.deploytodo.com/do-btn-blue.svg" width="240" alt="Deploy to DO"></a>


## Installation

To install MyKit, you'll want to clone or download this repo:

```
git clone https://github.com/aprunty41/MyKit.git project_name
```

Next, we can install MyKit with these **4 simple steps**:

### 1. Create a New Database

We'll need to utilize a MySQL database during the installation. For the following stage, you'll need to create a new database and preserve the credentials.

### 2. Copy the `.env.example` file

We need to specify our Environment variables for our application. You will see a file named `.env.example`, you will need to duplicate that file and rename it to `.env`.

Then, open up the `.env` file and update your *DB_DATABASE*, *DB_USERNAME*, and *DB_PASSWORD* in the appropriate fields. You will also want to update the *APP_URL* to the URL of your application.

```bash
APP_URL=http://mykit.test

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=mykit
DB_USERNAME=root
DB_PASSWORD=
```


### 3. Add Composer Dependencies

Following that, we'll need to install all composer dependencies through the following command:
```php
composer install
```
### 4. Run Migrations and Seeds

We must migrate our database schema into our database, which we can accomplish by running the following command:
```php
php artisan migrate
```
<br>
Finally, we will need to seed our database with the following command:

```php
php artisan db:seed
```
<br>
php artisan serve
 
 Your app will then be available in your local browser at http://127.0.0.1:8000
 
 
🎉 And that's it! You will now be able to visit your URL and see your Wave application up and running.



## Documentation

