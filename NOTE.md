docker images
docker pull hello-world
docker run hello-world

---

docker pull ubuntu:18.04
docker run ubuntu:18.04 -> 바로 종료가 됌
docker run -it ubuntu:18.04 /bin/bash

---

docker pull node:latest
docker run -it node:latest /bin/sh

<!-- docker look build image history -->
docker history sample-app:latest

<!-- rm option make delete in th container -->
docker run --rm -it ubuntu:latest /bin/bash

<!-- delete unnessesary files -->
docker container prune
docker image prune

<!-- remove images -->
docker image rm ${IMAGE_NAME}


docker exec -it ${CONTIAINER_ID} /bin/sh

docker container top ${CONTAINER_ID}

docker -f ${dockerfilename} -t ${image} .

<!-- run on port! -->
docker run -d -p 8080:8080 sample-app:latest



---
## docker compse

<!-- start -->
docker-compose up
docker-compose -f ${DOCKER_COMPOSE_FILENAME} up
<!-- stop -->
docker-compose down

