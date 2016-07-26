# STL Full Stack Web Development Website

**In Progress**

This is the website for the [Saint Louis Full Stack Web Development](https://www.meetup.com/SaintLouis_FullStack_WebDevelopment/events/231969178/) meetup group.

This project was started and will be mostly built out during the monthly hack nights.

At the moment, the plan is to build this website using:

- Laravel
- MySQL (though we may switch to postgres)
- Vue.js

## Required tools

To work on this project, you'll need the following tools installed on your computer:

- [PHP (at least version 5.5)](http://php.net/manual/en/install.php)
- [Composer](https://getcomposer.org/)
- [Node](https://nodejs.org/en/)
- [Git](https://git-scm.com/)
- [MySQL](http://dev.mysql.com/downloads/)

You'll also need some kind of web server. Since this is a laravel project I would suggest either:

- [Laravel Valet](https://laravel.com/docs/5.2/valet)
    - This is a simpler setup and does not involve setting up a virtual machine
- [Laravel Homestead](https://laravel.com/docs/5.2/homestead)

Either of these options will be a relativly easy setup. You could also use any other webserver or virual host you'd like to host the project. If you want to check out or work on the site quickly you can even turn on php's built in server via the commands:

    cd path/to/FullStackWebsite/public
    php -S localhost:8000
    open http://localhost:8000

## Getting up and running

Once you have the required tools installed, pull down the project from github with the following commands:

    cd path/to/location/you/want/to/store/the/project/in/
    git clone https://github.com/chris-schmitz/fullstack-website.git fullstack-website

This will pull the project down to your computer. After that you'll need to install the dependencies:

    cd fullstack-website/FullStackWebsite
    composer install

And create your `.env` file:

    cp .env-example .env

And update the `.env` file to reflect your development environment.

Once the dependencies have been installed and your `.env` file is updated, you just need to make sure your webserver is configured to use the `FullStackWebsite/public` directory as it's document root.