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
