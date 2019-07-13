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
  --no-dev        Do not install IDE Helper, Debug Bar end Extended Generators
  --no-helpers    Do not install Eloquent Sluggable, Eloquent Filter and Eloquent Sortable
  --no-graphql    Do not install Lighthouse
```
## Packages to be installed:
  * IDE Helper            : Generates a helper file for IDE
  * Debug Bar             : Integrates PHP Debug Bar
  * Extended Generators   : Extends built-in generators
  * Eloquent Sluggable    : Slugs for models
  * Eloquent Filter       : Filter models and relationships
  * Eloquent Sortable     : Sortable behaviour models
  * Lighthouse            : GraphQL library for Laravel
