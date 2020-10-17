# How-to

## Requiremenet
- [Docker](https://docs.docker.com/engine/install/ubuntu/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Run
```
docker-compose up -d

Creating network "ghost_ghost_network" with the default driver
Creating ghost_web_ghost_1 ... done
Creating ghost_database_1  ... done
```

## Verify
```
docker-compose ps
```

Output:
```
      Name                     Command               State           Ports         
-----------------------------------------------------------------------------------
ghost_database_1    docker-entrypoint.sh mysqld      Up      3306/tcp, 33060/tcp   
ghost_web_ghost_1   docker-entrypoint.sh node  ...   Up      0.0.0.0:8080->2368/tcp
```

## Testing
- Access url http://localhost:8080
- Admin url http://localhost:8080/ghost