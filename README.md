# docker_excersice
## 01.docker_basic

* docker ps [-a]
* docker container [ls] [-a]

* docker pull
* docker tag [image name]:[tag name] [hub id/new image name]:[tag name]  
  - 자신의 허브 계정 아이디와 일치해야 push 가능
* docker push

* docker commit  
이미지 레이어 반영 (변경된 내용을 새로운 컨테이너에 반영)
* .dockerignore  
  - 컨테이너 빌드시 포함하지 않을 파일 명시
* docker build -t [tag name] -f [image name] . (Dockerfile directory)
* docker run --name [container name] -d (background) -p (port) (host:dst) [image name:tag name]
* docker stop / restart 

* docker attch [container name]  
  - 백그라운드로 실행되고 있는 컨테이너의 로그를 확인 (포그라운드)
* docker exec -it [container id] /bin/bash  
  - 컨테이너를 실행시킴과 동시에 배쉬창 활성화

* docker logs [container name]
* docker rm [container id]
* docker rmi [image id]
