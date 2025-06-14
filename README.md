<p align="center">
<img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo">
<img src="https://raw.githubusercontent.com/bigskysoftware/htmx/f690d928342b6334fa539cfbd4be515748d2ba0f/www/static/img/htmx_logo.2.png" width="200" alt="HTMX Logo">
</p>

# Laravel HTMX Starter Kit

A heavily opinionated starter kit for Laravel that bundles essential tooling with the simplicity of HTMX into a jumping off point.

## Requirements

- PHP 8.4
- [Bun](https://bun.sh/) (Can be replaced with your package manager of choice, see below)

## Installed Packages

The following packages come pre-installed:

- [Htmx](https://htmx.org)
- [Lefthook](https://lefthook.dev)
- [Octane](https://laravel.com/docs/octane)
  - [FrankenPHP](https://frankenphp.dev)
- [Pest](https://pestphp.com)
  - [Arch Plugin](https://pestphp.com/docs/arch-testing)
  - [Laravel Plugin](https://pestphp.com/docs/plugins#laravel)
- [PHPStan](https://phpstan.org)
  - [Larastan](https://github.com/larastan/larastan)
- [Pint](https://laravel.com/docs/pint)
- [Prettier](https://prettier.io)
- [Rector](https://getrector.com)

### Pint

The Pint config is based on [Nuno Maduro's Essentials package](https://github.com/nunomaduro/essentials) with some tweaks:

- Uses PER preset
- [Groups Imports](https://cs.symfony.com/doc/rules/import/group_import.html)
  - By extension, disables [Single Import Per Statement](https://cs.symfony.com/doc/rules/import/single_import_per_statement.html)
- [New With Parenthesis](https://cs.symfony.com/doc/rules/operator/new_with_parentheses.html)
  - Disabled for anonymous classes
- [No Unused Imports](https://cs.symfony.com/doc/rules/import/no_unused_imports.html)
- [Yoda Style](https://cs.symfony.com/doc/rules/control_structure/yoda_style.html)

### PHPStan

By default, PHPStan is set to level 10.

### Bun

By default, this starter kit uses [Bun](https://bun.sh) to manage JavaScript dependencies. If you prefer to use a different one, do the following:

- Delete `bun.lock`
- Update `bun` references with the equivalent of your preferred package manager in:
  - `composer.json`
  - `lefthook.yaml`
  - `maskfile.md`
  - `package.json`
- Delete the `node_modules` folder
- Reinstall your JavaScript dependencies

## Common Scripts

Common scripts as handled using [Mask](https://github.com/jacobdeichert/mask).

While these are useful, you're not required to have Mask installed.
