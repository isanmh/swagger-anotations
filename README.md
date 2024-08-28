Install Packages Swagger Laravel:
```
composer require "darkaonline/l5-swagger"
```
You can publish L5-Swagger's config and view files into your project by running:
```
php artisan vendor:publish --provider "L5Swagger\L5SwaggerServiceProvider"
php artisan l5-swagger:generate
```
Open your AppServiceProvider (located in app/Providers) and add this line in register function :
```
$this->app->register(\L5Swagger\L5SwaggerServiceProvider::class);
```
