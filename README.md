# Startup Winter CMS Theme

This is an altered version of the basic theme created by [Winter CMS Scaffolding](https://wintercms.com/docs/v1.2/docs/console/scaffolding).

### Tailwind

[Tailwind CSS](https://tailwindcss.com/) has been upgraded to version 4

### Vite

The vite config includes setup to hot reload the browser upon saving changes.

## How to install

From root of project, run:
```sh
composer require funkduk/wn-startup-theme
```

## Development

The theme is built on Tailwind CSS, which is built using the NodeJS framework. To be able to compile any changes made to the styling or content, you must use the vite commands that are included with  [Winter CMS Asset Compilation (vite)](https://wintercms.com/docs/v1.2/docs/console/asset-compilation-vite).

#### You must first install the Node dependencies required for the theme.

`php artisan vite:install -p theme-startup`

#### Then, to compile the Tailwind CSS styles for development, run the following command in the root folder of the project:

`php artisan vite:compile -p theme-startup`

#### To compile the Tailwind CSS styles for production (which should be done if you commit any changes to the Workshop theme), you must add the --production flag to the above command:

`php artisan vite:compile -p theme-startup --production`

#### To make it easy to develop the theme, you can also watch the necessary template and stylesheet files for any changes:

`php artisan vite:watch theme-startup`
