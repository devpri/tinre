## About Tinre

Open Source URL Shortener built with Laravel.

## Installation

1. Run `composer create-project devpri/tinre`.
2. Update the `DB_*` variables in `.env`. After that run `php artisan migrate` to create all tables.
3. Run `php artisan user:create` to create the first user.
4. Run `php artisan tinre:publish` to publish the assets.
5. Get a [MaxMind](https://support.maxmind.com/account-faq/license-keys/how-do-i-generate-a-license-key/) license key and update the `MAXMIND_LICENSE_KEY` variable. After that run `php artisan geoip:update` to update the GeoIP database.
6. Update the `MAIL_*` variables in .env.

## Security

If you discover a security vulnerability, please send an e-mail to [paul@devpri.com](mailto:paul@devpri.com).

## License

Tinre is open-source software licensed under the [MIT License](https://github.com/devpri/tinre/blob/master/LICENSE.md).