#INSTRUCTION

### <span style="color:lightblue">1. Установка зависимостей</span>

Для того, чтобы установить зависимости нужно запустить

<span style="color:white">
docker run --rm \
-u "$(id -u):$(id -g)" \
-v $(pwd):/var/www/html \
-w /var/www/html \
laravelsail/php80-composer:latest \
composer install --ignore-platform-reqs
</span>

### <span style="color:lightblue">2. Генерация ключа</span>

<span style="color:white"> ./vendor/bin/sail php artisan key:generate </span>
### <span style="color:lightblue">3. Запуск </span>

<span style="color:white"> ./vendor/bin/sail up </span>

или

установить алиас <span style="color:white"> alias sail="./vendor/bin/sail" </span> и запустить <span style="color:white"> sail up </span>


- [Подробнее](https://laravel.com/docs/8.x/sail#installing-composer-dependencies-for-existing-projects).
- [Sail](https://laravel.com/docs/8.x/sail).
