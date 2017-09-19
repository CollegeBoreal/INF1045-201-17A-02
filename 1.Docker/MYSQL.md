# Docker

. Installer MySQL

```
$ docker run --name some-mysql -e MYSQL_ROOT_PASSWORD=password -p 3306:3306 -d mysql:latest 
```

. Executer la commande d'accer a MySQL

```
$ docker exec -it some-mysql bash
```
