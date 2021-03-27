# DOCKER COMPOSE PHPMYADMIN MYSQL

Compose is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration. 

Learn more docker compose <a href="https://docs.docker.com/compose/overview/" target="_blank">here</a>


> This repo is used for starter user to deploy mysql and phpmyadmin easy.

## Playground

1. Clone this repository
```
    git clone git@github.com:fuadajip/dockercompose-mysql-phpmyadmin.git
```

2. Change to directory
```shell
    cd dockercompose-mysql-phpmyadmin
```
3. Up the compose
```
    docker-compose up -d
```
4. Access phpmyadmin
[your_ip:8183](http://127.0.0.1:8183/)

5. Access mysql on terminal
```
    docker exec -it dev_mysql mysql -u root -p
```

## Change Root password
For this you must set `MYSQL_PASSWORD` variable.

1. make `.env` file in project directory and paste these value on that
```
MYSQL_PASSWORD=changeme
```

## For more information about phpmyadmin image
<a href="https://hub.docker.com/r/phpmyadmin/phpmyadmin/" target="_blank">READ HERE</a>

## For more information about mysql ENV
<a href="https://hub.docker.com/_/mysql/" target="_blank">READ HERE</a>
