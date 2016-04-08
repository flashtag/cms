![Flashtag](https://s3-us-west-2.amazonaws.com/flashtag/images/flashtag-logo-banner.png)

## Flashtag CMS

Standalone install of Flashtag CMS

- [Wiki](https://github.com/flashtag/flashtag/wiki)
- [Issues](https://github.com/flashtag/flashtag/issues)

### Installation

```
composer create-project "flashtag/cms:dev-master@dev" flashtag --prefer-dist
```

### Dev environment - Homestead

If you have Vagrant installed

1. run `vendor/bin/homestead make` and modify `Homestead.yaml` to suit your needs
2. run `vagrant up`
3. run `vagrant ssh` and cd to your project directory and run `php artisan flashtag:install`.

Everything should be good.


### Production

- Clone your project repository and run `composer install`
- Copy `.env.example` to `.env` and set it up as required. Don't forget to change `APP_ENV` to `production` and `APP_DEBUG` to `false`.
- Generate your key `php artisan key:generate`
- Set `JWT_SECRET` to a random string.
- Run the install script. `php artisan flashtag:install`

Everything should be good.


### About

Tired of convoluted CMS interfaces that try to do everything through the dashboard or with modules that would best be left to a developer to do?

Flashtag is a new CMS aimed to cause you the least amount of stress. We embrace our PHP framework and try to keep everything as vanilla as possible.

![Posts index](https://s3-us-west-2.amazonaws.com/flashtag/screenshots/alpha/admin-posts-index.png)

