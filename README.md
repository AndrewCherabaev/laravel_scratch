# Laravel Scratch
Creates Laravel 5 project with awesome packages

## Use

```
php laravel_scratch --name=project_name
```

Options:
```
  -h, --help      Show help message
  --name=project  Required. Name of new project
        
  --pure          Do not install additional packages
```
## Packages to be installed:
  * [IDE Helper](https://github.com/barryvdh/laravel-ide-helper) - Generates a helper file for IDE auto-completion
  * [Debug Bar](https://github.com/barryvdh/laravel-debugbar) - Integrates PHP Debug Bar with Laravel
  * [Laravel 5 Extended Generators](https://github.com/laracasts/Laravel-5-Generators-Extended) - Extends built-in file generators
  * [Eloquent Sluggable](https://github.com/cviebrock/eloquent-sluggable) - Create slugs for Eloquent models
  * [Eloquent Filter](https://github.com/Tucker-Eric/EloquentFilter) - Filter models and their Relationships
  * [Eloquent Sortable](https://github.com/spatie/eloquent-sortable) - Sortable behaviour for Eloquent models
  * [Laravel Breadcrumbs](https://github.com/davejamesmiller/laravel-breadcrumbs) - Create and manage breadcrumbs
  * [Lighthouse](https://github.com/nuwave/lighthouse) - An up and coming GraphQL library for Laravel

  Special thanks to [Awesome Laravel](https://github.com/chiraggude/awesome-laravel)

## About `scratch.json`

```json
{
  "name": Name of package, ie "Lighthouse",
  "description": Description text for help message,
  "composer": Name of composer repo "nuwave/lighthouse",
  "artisan": [ 
      List of specific artisan connads to be run
      "vendor:publish --provider=\"Nuwave\\Lighthouse\\LighthouseServiceProvider\" --tag=schema",
      "vendor:publish --provider=\"Nuwave\\Lighthouse\\LighthouseServiceProvider\" --tag=config"
  ]
}
```

## Todo
* ~~Add `scratch.json` for easy packages list modifying~~
* ~~Remove some flags~~
* Add some another awesome packages
* Add links to ~~packages repositories and Laravel Awesome list~~
