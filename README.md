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
  --no-laravel    Do not create project, just add packages

  --test          Do nothing but you can see result imidiately
```

**Important!** For *nix only! If you use Windows, you can run it inside Vagrant

## Packages to be installed:
  * [Doctrine DBAL](https://github.com/doctrine/dbal) - Powerful database abstraction layer. Uses in `ALTER COLUMN` migrations 
  * [IDE Helper](https://github.com/barryvdh/laravel-ide-helper) - Generates a helper file for IDE auto-completion
  * [Debug Bar](https://github.com/barryvdh/laravel-debugbar) - Integrates PHP Debug Bar with Laravel
  * [Laravel 5 Extended Generators](https://github.com/laracasts/Laravel-5-Generators-Extended) - Extends built-in file generators
  * [Laravel Activitylog](https://github.com/spatie/laravel-activitylog) - Log activity inside your Laravel app
  * [Eloquent Sluggable](https://github.com/cviebrock/eloquent-sluggable) - Create slugs for Eloquent models
  * [Eloquent Filter](https://github.com/Tucker-Eric/EloquentFilter) - Filter models and their Relationships
  * [Eloquent Sortable](https://github.com/spatie/eloquent-sortable) - Sortable behaviour for Eloquent models
  * [Laravel AdminLTE](https://github.com/jeroennoten/Laravel-AdminLTE) - AdminLTE integration with Laravel (disabled by default)
  * [Laravel Menu](https://github.com/spatie/laravel-menu) - Html Menu Generator (disabled by default)
  * [Laravel Breadcrumbs](https://github.com/davejamesmiller/laravel-breadcrumbs) - Create and manage breadcrumbs (disabled by default)
  * [Lighthouse](https://github.com/nuwave/lighthouse) - An up and coming GraphQL library for Laravel
  * [Laravel CORS](https://github.com/barryvdh/laravel-cors) - CORS Middleware for Laravel 5

  Special thanks to [Awesome Laravel](https://github.com/chiraggude/awesome-laravel), [Spatie team](https://github.com/spatie)
and [Barry vd. Heuvel](https://github.com/barryvdh)
## About `scratch.json`

```js
{
  //Name of package
  "name": "Lighthouse",
  //Description text for help message
  "description": "GraphQL library for Laravel",
  // Name of composer repo 
  "composer": "nuwave/lighthouse",
  //List of specific commands to be run
  "commands": [ 
    "php artisan vendor:publish --provider=\"Nuwave\\Lighthouse\\LighthouseServiceProvider\" --tag=schema",
    "php artisan vendor:publish --provider=\"Nuwave\\Lighthouse\\LighthouseServiceProvider\" --tag=config"
  ],
  //Set to true if you need not to install this package
  "ignore": false 
}
```

## Todo
* Add some another awesome packages
* ~~Remove some flags~~
* ~~Add `scratch.json` for easy packages list modifying~~
* ~~Add links to packages repositories and Laravel Awesome list~~

## Installation perfomance
Installation checked for all packages (13 + laravel/framework), even they are disabled by default

```
Creating new Laravel 5 project 'test_perfomance'...

Install Laravel:             Done ✓
 + config (1/1):             Done ✓
Install Doctrine DBAL:       Done ✓
Install IDE Helper:          Done ✓
 + config (1/3):             Done ✓
 + config (2/3):             Done ✓
 + config (3/3):             Done ✓
Install Debug Bar:           Done ✓
 + config (1/1):             Done ✓
Install Extended Generators: Done ✓
Install Activitylog:         Done ✓
 + config (1/2):             Done ✓
 + config (2/2):             Done ✓
Install Eloquent Sluggable:  Done ✓
 + config (1/1):             Done ✓
Install Eloquent Filter:     Done ✓
 + config (1/1):             Done ✓
Install Eloquent Sortable:   Done ✓
Install Laravel-AdminLTE:    Done ✓ [disabled by default]
 + config (1/1):             Done ✓
Install Laravel Menu:        Done ✓ [disabled by default]
Install Breadcrumbs:         Done ✓ [disabled by default]
 + config (1/1):             Done ✓
Install Lighthouse:          Done ✓
 + config (1/2):             Done ✓
 + config (2/2):             Done ✓
Install Laravel CORS:        Done ✓ 
 + config (1/1):             Done ✓

Laravel 5 project 'test_perfomance' successfully created in 4:51 min
```

Installation under Linux (Debian 9, Core i5-7400, 16 GB RAM) took ~5 minutes

Installation under Windows (Vagrant Homestead, Core i7-7700, 4 GB RAM) took ~8 minutes

