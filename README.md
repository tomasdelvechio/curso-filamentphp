# Curso Filament 3 - Laravel

[URL de la playlist](https://www.youtube.com/playlist?list=PLVj5uXWMQ4cx-gORGvryMpk4TSyatO15t)

# Comandos por video

El curso asume PHP y composer instalado.

## Video 1

```bash
cd ~/workspace/
sudo apt install libapache2-mod-php8.1 php8.1 php8.1-cli php8.1-curl php8.1-opcache php8.1-readline php8.1-xml php8.1-sqlite3 php8.1-pgsql php8.1-mysql php8.1-intl php8.1-zip
composer create-project laravel/laravel curso-filamentphp
composer require livewire/livewire
composer require filament/filament:"^3.2" -W
git init
git branch -m main
```

## Video 4

```bash
php artisan migrate
php artisan make:filament-user
php artisan vendor:publish --tag=filament-config
php artisan make:model Category -m
php artisan make:model Brand -m
php artisan make:model Product -m
php artisan make:model Customer -m
php artisan make:model Order -m
```

## Video 5

```bash
php artisan make:model OrderItem -m
php artisan make:migration create_category_product_table

# Hacer los pasos del video y al final del mismo
php artisan migrate
```

## Video 6

```bash
php artisan make:filament-resource Product

php artisan storage:link
```

Si se usa artisan como servidor, en necesario modificar el archivo `.env`

```
APP_URL=http://127.0.0.1:8000
```

Poner la url que corresponda (ver si se ejecuta con sail, etc...)

## Video 13

```bash
php artisan make:filament-resource Brand
```