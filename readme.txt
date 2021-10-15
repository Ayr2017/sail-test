1. Для того, чтобы установить зависимости нужно запустить

docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php80-composer:latest \
    composer install --ignore-platform-reqs

2. Установить ключ

./vendor/bin/sail php artisan key:generate
