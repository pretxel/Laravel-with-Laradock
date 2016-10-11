# Laravel 5.3 with Laradock

## Installation

### Init submodule

```javascript
git submodule init
git submodule update
```
### Create containers

```javascript
cd laradock
docker-compose up -d nginx mysql phpmysql redis
```

### Run commands inside workspace container

```javascript
docker exec -it laradock_workspace_1 bash
composer install
php artisan key:generate
php artisan migrate
```

### Run
[http://localhost/](http://localhost/)