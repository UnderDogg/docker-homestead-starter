# laravel-docker

PHP7-FPM, NGINX, MySQL for developing Laravel application

    $ git clone git@github.com:taras-by/laravel-docker.git
    $ cd laravel-docker
    $ docker-compose build
    $ docker-compose up -d
    $ docker-compose exec --user="www-data" app composer install

Run application: http://localhost:835
