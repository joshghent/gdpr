web: vendor/bin/heroku-php-apache2 public/
worker: php artisan queue:listen --tries=10 --delay=20
release: composer install --optimize-autoloader && php artisan config:cache