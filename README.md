# Frontend Starter

[Laravel Elixer](http://laravel.com/docs/5.1/elixir) is a powerful tool built with Glup enhancement.
It's easy of use for all frontend developers.

This starter package is for quickly setup and use in any web project.

Simply clone the starter package, and get ready to build frontend files.

## Installation & Setup

### Install Node

Node.js is must have tool.

Download and install from <https://nodejs.org>

### Install Gulp (global install)

    npm install --global gulp

### Install Laravel Elixir

Essential packages are already defined in `package.json`.

Just run:

    npm install

For Windows user:

    npm install --no-bin-links

## Execute Elixer

Run all tasks

    gulp

Run all tasks and minify all CSS and JavaScript

    gulp --production

Watch for changes

    gulp watch

## Elixer Usage

Compile Sass into CSS. Default sass folder: `resources/assets/sass`.

```
elixir(function(mix) {
    mix.sass('app.scss');
});
```

Compile multiple Sass files into a single CSS file, and customize the output directory:

```
elixir(function(mix) {
    mix.sass([
        'app.scss',
        'page.scss'
    ], 'public/assets/css');
});
```

More elixer usage: <http://laravel.com/docs/5.1/elixir>