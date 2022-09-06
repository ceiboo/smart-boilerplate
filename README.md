# Smart Boiler Plate
Sistema base para proyectos

### Instalación ###
* `docker-compose build smartapi`
* `docker-compose up -d`

### Si necesitamos anexar laravel ###
* `docker-compose exec smartapi composer create-project --prefer-dist laravel/laravel / "9.0.*`

### Si ya tenemos laravel ###
* `docker-compose exec smartapi composer update`
* `docker-compose exec smartapi php artisan key:generate`

### Crear estructura de datos ###
* `docker-compose exec ceiboo-cms php artisan migrate:fresh`


### Otros comandos ###
Para bajar los dockers
* `docker-compose down`

### Para tener acceso al endpoint del docker a la app ###
En tu archivo /etc/hosts incluir las siguientes lineas
* `127.0.0.1 api.smartsignane.smw`

- Test de instalación en navegador:
* `http://api.smartsignane.smw/`
