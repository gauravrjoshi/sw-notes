# [Testing: Getting Started](https://laravel.com/docs/11.x/testing)

## Introduction

By default, your application's tests directory contains two directories:

1. Feature Testing
2. Unit Testing

### Unit Testing:

Unit tests are tests that focus on a very small, isolated portion of your code. In fact, most unit tests probably focus
on a single method. Tests within your "Unit" test directory do not boot your Laravel application and therefore are
unable to access your application's database or other framework services.

### Feature Testing:

Feature tests may test a larger portion of your code, including how several objects interact with each other or even a
full HTTP request to a `JSON` endpoint. Generally, most of your tests should be feature tests. These types of tests
provide the most confidence that your system as a whole is functioning as intended.


An `ExampleTest.php` file is provided in both the Feature and Unit test directories. After installing a new Laravel application, execute the `vendor/bin/pest`, `vendor/bin/phpunit`, or `php artisan test` commands to run your tests.

## Environment

When running tests, Laravel will automatically set the configuration environment to testing because of the environment variables defined in the `phpunit.xml` file. Laravel also automatically configures the session and cache to the `array` driver so that no session or cache data will be persisted while testing.
