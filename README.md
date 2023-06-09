## Iniciando projeto com [spring boot](https://github.com/FranciscoWallison/abctechapi_11AOJO)

## Projetos
[api](https://github.com/FranciscoWallison/abctechapi_11AOJO)
[app](https://github.com/FranciscoWallison/abc_tech_app_11aojo)

### [mvnrepository](https://mvnrepository.com/)


## Possiveis erros

Validar erro de './mvnw: not found' ou  './commands.sh: not found' 

````
sudo dos2unix mvnw && chmod +x mvnw
sudo dos2unix commands.sh && chmod +x commands.sh
````
### Comando para entrar no container do app
````
docker exec -it api bash
````
### Comando para reiniciar os containers
````
sudo docker compose -f "docker-compose.yml" down && docker compose -f "docker-compose.yml" up -d --build
````

### Comandos básicos MYSQL
````
mysql -uroot -pFiap1234;
show databases;
show tables;
````

### Comandos básicos sql
````
USE abc_tech;
select * from assistances;
select * from flyway_schema_history;
select * from order_location;
select * from orders;
select * from orders_assists;
````

### ENV
````
./mvnw spring-boot:run -Dspring-boot.run.jvmArguments="-DDB_HOSTNAME=db_mysql -DDB_PORT=3306 -DDB_NAME=abc_tech -DDB_USERNAME=root -DDB_PASSWORD=Fiap1234"
````


### Amazon RDS
````
Utilizando Mysql
````
