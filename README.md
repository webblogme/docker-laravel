# Docker Laravel Starter Pack

Build a website with Laravel

### Package include
* [Laravel](https://laravel.com/) - PHP Framework For Web Artisans v 5.4.30

### Built With DOCKER
* PHP 5.6

### Requirement
You should have these install on your machine
* Docker version 18.03
* Composer
* node v9.3.0
* Git

### Tested on 
* Windows 7
* Docker runs with Oracle VM

### How to use
Run docker machine.
In case of first time use: you need to run command in MINGW64
```
docker-compose build
```
then you can just type in cmd 
```
docker-compose up -d
```

### To access PHP MyAdmin
```
http://localhost:8888
```
Username: root / Password: root

### To do after run docker-compose

```
composer create-project --prefer-dist laravel/laravel laravel5 "5.4.30"
cd laravel5
composer require barryvdh/laravel-debugbar --dev
php artisan vendor:publish --provider="Barryvdh\Debugbar\ServiceProvider"
php artisan make:auth
```



### Enjoy coding!