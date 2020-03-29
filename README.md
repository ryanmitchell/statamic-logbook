# Logbook

**View log files in the CP**

Viewing log files directly on the server can be a bit of a hassle... First you have to `ssh` in, `cd` to the project's logs directory, and finally open each one only to see the biggest mangle of info logs and error logs with stack traces.

Logbook solves this by displaying each log file in a table and collapsing the stack traces to keep things nice and tidy.
You can view a full stack trace by clicking on it.

![logbook](https://user-images.githubusercontent.com/5065331/37864552-1983d97c-2f71-11e8-8011-3e430e5985ba.png)

## Installation

Install the addon via composer:

```
composer require aryehraber/statamic-logbook:dev-statamic-3
```

Publish the utility assets:

```
php artisan vendor:publish --provider="AryehRaber\Logbook\LogbookServiceProvider"
```

That's it! Logbook can now be accessed via the CP under `Tools > Utilities`.
