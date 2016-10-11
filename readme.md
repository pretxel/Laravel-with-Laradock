# Laravel 5.3 with Laradock

## Installation

### Init submodule

``bash
git submodule init
git submodule update
``
### Create containers

``bash
cd laradock
docker-compose up -d nginx mysql phpmysql redis
``

### Run commands inside workspace container

``bash
docker exec -it laradock_workspace_1 bash
composer install
php artisan key:generate
php artisan migrate
``

### Run
[http://localhost/](http://localhost/)