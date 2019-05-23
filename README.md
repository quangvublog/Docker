# Docker Simple


To list any running containers 

$ docker ps
CONTAINER ID  IMAGE  COMMAND  CREATED  STATUS  PORTS  NAMES
<I do not have have any running right now>
  
To kill a container

$ docker kill <CONTAINER ID>
  
To see if you have any containers even if they are not running.  

$ docker images
REPOSITORY               TAG     IMAGE ID      CREATED       SIZE
mtngt/angular_docker  latest  ec5a8c5f01f1  2 hours ago   17MB

To clear out all the not running stuff as well
$ docker system prune -a

To build a docker image
$ docker build -t simple:latest .

To run the build

$ docker run -d -p 5000:5000 simple:latest

To push image to Docker Hub

Login from terminal
$ docker login -u quangvublog
Password:

Login Succeeded

To retag image 
$ docker tag simple quangvublog/my_docker_flask

To push
$ docker push quangvublog/my_docker_flask

To pull
$ docker pull quangvublog/my_docker_flask

source: <a href="https://blog.vu-review.com">blog công nghệ</a>
