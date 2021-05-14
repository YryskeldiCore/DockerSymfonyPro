docker commands and their meanings

1)docker exec -it php74-container bash - "go to console of php container and install whatever you want"

docker exec -it mariadb-container bash - same command like upper but using mariadb

you can sign in typing the login and password to DB
and use all cmds of MariaDB

2)docker-compose run --rm node-service yarn install - "Launching docker utility, removing node-service and run the cmd yarn install"

FE:
docker-compose run --rm php74-service php bin/console doctrine:database:create - "It's the alternative to docker exec cmd"
Remember that you can't install directly from the console you need to log in to container terminal

1)docker exec -it php74-container bash
2)docker-compose run --rm php74-service composer require symfony/maker-bundle

and then you need to always work inside of this terminal using create-entity and something like this

3)docker-composer up -d --build - "Building the docker container"