https://github.com/ProgrammerZamanNow/belajar-docker-compose

# docker compose create
    create container from docker-compose.yaml file in our current working directory

# docker compose start
    start/run container that we create before

# docker compose ls
    show all containers from the compose file

# docker compose stop
    stops the container from the compose file, but does not remove/delete it
    use docker compose stop containerName for stop the desired container

# docker compose up
    start and run containers, shortcut for docker compose create && docker compose start
    use -d for detach mode

# docker compose down
    stop and delete containers, network, and volume.