# A tool to allow BelongsTo searchable fields to be pre-populated with data

This is a continuation of the https://github.com/alexbowers/nova-prepopulate-searchable package. The reason for the clone is that at the time of the cloning of the package, the original package has not been maintained as was causing errors.

## Installation

You can install the package in to a Laravel app that uses [Nova](https://nova.laravel.com) via composer:

```sh
composer require genealabs/nova-prepopulate-searchable
```

## Usage

On any `BelongsTo` fields in your resources that are `searchable()`, you can also add `prepopulate()` to the method chain and the field will be prepopulated with values to choose from.

You may optionally pass through a search query to the prepopulate method, and the keywords passed will be used for
the search initially, before resetting the search to being empty (as it currently is).

![Prepopulate Search](https://github.com/genealabs/nova-prepopulate-searchable/blob/master/screenshots/example.gif?raw=true)
