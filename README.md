<p align="center">
    <a href="https://www.mangoweb.cz/en/" target="_blank">
        <img src="https://avatars0.githubusercontent.com/u/38423357?s=200&v=4"/>
    </a>
</p>
<h1 align="center">Shipping packing slips</h1>

## Features

xxxx

## Installation

1. Run `$ composer require mangoweb-sylius/sylius-packing-slips-plugin`.
2. Register `\MangoSylius\PackingSlipsPlugin\MangoSyliusPackingSlipsPlugin` in your Kernel.
3. Import `@MangoSyliusPackingSlipsPlugin/Resources/config/routing.yml` in the routing.yml.

```
mango_sylius_shipment_export_plugin:
    resource: "@MangoSyliusPackingSlipsPlugin/Resources/config/routing.yml"
    prefix: /admin
```

### Usage

You can override package slips grid template.

* `@MangoSyliusPackingSlipsPlugin/show.html.twig`
* `@MangoSyliusPackingSlipsPlugin/tdUnit.html.twig`

## Development

### Usage

- Create symlink from .env.dist to .env or create your own .env file
- Develop your plugin in `/src`
- See `bin/` for useful commands

### Testing

After your changes you must ensure that the tests are still passing.
* Easy Coding Standard
  ```bash
  bin/ecs.sh
  ```
* PHPStan
  ```bash
  bin/phpstan.sh
  ```
License
-------
This library is under the MIT license.

Credits
-------
Developed by [manGoweb](https://www.mangoweb.eu/).