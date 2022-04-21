# How to setup
``` bash
git clone <your_project> source
cp .env.example .env
cp .env.source.example ./source/.env

docker-compose up --build -d
docker-compose run --rm composer install
docker-compose run --rm artisan key:generate
docker-compose run --rm artisan migrate:fresh --seed
```
# Ports location
``` txt
localhost:8080 - project
localhost:8081 - phpmyadmin
localhost:8082 - mongodb express
localhost:8083 - redis commander
```