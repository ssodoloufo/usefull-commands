# Usefull DevOps Commands

## Nginx

```[nginx]
- To disable autoload apache service, run : 
    `sudo systemctl disable apache2`
- To stop apache service, run : 
    `sudo /etc/init.d/apache2 stop`
- To start nginx service, run : 
    `sudo systemctl restart nginx`
```

## Docker

```[docker]
BUILD AN DOCKER IMAGE ----> sudo docker compose up -d --build
SHOW DOCKER AVAILABLE IMAGES ----> sudo docker images
REMOVE AN DOCKER IMAGE ----> sudo docker rmi cff6b68a194a

----> LARAVEL DOCKER COMMANDS
 sudo docker compose exec app chmod -R gu+w bootstrap storage public
 sudo docker compose exec app chmod -R guo+w bootstrap storage public
 sudo docker compose exec app composer install
 sudo docker compose exec app composer dump-autoload
 sudo docker compose exec app php artisan migrate --seed

----> REMOVE ALL AVAILABLE IMAGE
 sudo docker image ls -f "dangling=true"
 sudo docker image prune -a -f
 sudo docker system prune -a --volumes -f

----> ADD AVAILABLE IMAGE TO DOCKERHUB
 sudo docker run --rm -it ssodoloufo/laravel-training-web
 sudo docker tag digit-laravel-training-app ssodoloufo/laravel-training-web
 sudo docker push ssodoloufo/laravel-training-web
```

## Laravel

```[laravel]

```
