<p align="center"><img src="http://media.devpri.com/tinre/logo.png" width="300"></p>

<p align="center">
<a href="https://github.com/devpri/tinre-core/actions"><img alt="GitHub Tests" src="https://github.com/devpri/tinre-core/workflows/tests/badge.svg"></a>
<a href="https://scrutinizer-ci.com/g/devpri/tinre-core/"><img alt="Scrutinizer code quality" src="https://img.shields.io/scrutinizer/quality/g/devpri/tinre-core/master"></a>
<a href="https://github.styleci.io/repos/285526567"><img alt="StyleCI" src="https://github.styleci.io/repos/285526567/shield"></a>
<a href="https://packagist.org/packages/devpri/tinre"><img alt="Packagist" src="https://poser.pugx.org/devpri/tinre/v"></a>
<a href="https://github.com/devpri/tinre/blob/master/LICENSE.md"><img alt="GitHub" src="https://img.shields.io/github/license/devpri/tinre"></a>
</p>

## About Tinre

A fast and powerful URL Shortener built with Laravel, VueJS, and Tailwind CSS.

![Tinre](http://media.devpri.com/tinre/tinre.gif)

## Requirements
* PHP 7.3+
* Nginx or Apache
* MySQL, MariaDB or PostgreSQL
* Composer

## Installation

1. Run `composer create-project devpri/tinre`.
2. Update the `DB_*` variables in `.env`. After that run `php artisan migrate` to create all tables.
3. Run `php artisan user:create` to create the first user.
4. Run `php artisan tinre:publish` to publish the assets.
5. Get a [MaxMind](https://support.maxmind.com/account-faq/license-keys/how-do-i-generate-a-license-key/) license key and update the `MAXMIND_LICENSE_KEY` variable. After that run `php artisan geoip:update` to update the GeoIP database.
6. Update the `MAIL_*` variables in .env.

## Update

1. Make a backup of your data before updating.
2. Run `composer update` to update the dependencies.
3. Run `php artisan tinre:publish` to publish the assets.
4. Check and update [tinre-core](https://github.com/devpri/tinre-core) overridden files.

## Security

If you discover a security vulnerability, please send an e-mail to [paul@devpri.com](mailto:paul@devpri.com).

## License

Tinre is open-source software licensed under the [MIT License](https://github.com/devpri/tinre/blob/master/LICENSE.md).
