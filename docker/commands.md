# docker pull
pull or download docker image from repository, ex: hub.docker.com

# docker run
  2.1. docker run image:tag
    run docker image with attach mode
  2.2. docker run -d image:tag
   run image with detach mode, so we can close the terminal

# docker run -d -p 33061:3306 --name redis_latest -e ENV mysql:latest
   run latest version of mysql image.
   -p publish it's ports to 33061
   -d detach mode
   -e env if any
   --name / -n to rename container

# docker ps / docker ps -a
   show all container list, use -a to show all container including stopped/exited container

# docker start container_name/container_id
# docker stop container_name/container_id

# docker exec -it container_name/container_id
  log in to the container/server.
  -it interactive
  bash/sh so we can run commands

# docker logs -f container_name/container_id
  show logs of container, -f used to show live tail of logs

# docker images
  show all images on host

# docker build -t image_name:version .
  docker build -t todolist:v1
  will create docker image with name todolist and tag v1
