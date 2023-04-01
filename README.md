# Laravel schema builder
![schema-builder](./doc/schema-builder.png?raw=true "schema-builder")

Database designer & migration generator package for Laravel.

Checkout **[agontuk.github.io/schema-designer](https://agontuk.github.io/schema-designer)** to see how it works.

## Installation
Add at the bottom of your `composer.json`:
```json
    "prefer-stable": true, // add a comma to this line
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/J87NL/schema-builder"
        }
    ]
} // leave this existing closing tag
```
Run in your console to install:
```cli
composer require --dev j87nl/schema-builder:dev-main
```

Finally enable required routes via `.env`,
```php
SCHEMA_ROUTES_ENABLED=true
```
> NOTE: APP_ENV should be `local` to use this package.

## Usage
Navigate to `yoursite.com/schema` and build your database schema, then use the export button to generate migration files.

> NOTE: Not all features of migration are supported yet. Feel free to submit any issues or pull requests.

## License
[MIT](https://github.com/J87NL/schema-builder/blob/main/LICENSE)
