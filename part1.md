# 1.1
## docker container ps -a
CONTAINER ID        IMAGE                  COMMAND                  CREATED              STATUS                      PORTS                    NAMES
18124e2df8a7        nginx                  "nginx -g 'daemon of…"   About a minute ago   Exited (0) 29 seconds ago                            strange_brown
e9ce9d9b43fa        eetuh/dockertraining   "npm start"              2 minutes ago        Exited (0) 7 seconds ago                             pedantic_panini
123f3abc6a01        eetuh/eetuhakkinen     "npm start"              8 days ago           Up 24 minutes               0.0.0.0:8080->8080/tcp   elegant_williams
b849efcd28b7        eetuh/eetuhakkinen     "npm start"              8 days ago           Exited (128) 8 days ago                              romantic_proskuriakova

# 1.2
## docker ps -a
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

## docker images
REPOSITORY           TAG                 IMAGE ID            CREATED             SIZE

# 1.3
## commands
docker run -it devopsdockeruh/pull_exercise

password: basics
Secret message: "This is the secret message"

# 1.4
docker run devopsdockeruh/exec_bash_exercise
Secret message: "This is the secret message"

# 1.5
sudo docker run -it ubuntu:16.04 sh -c 'apt-get update; apt-get install curl; echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'

Input website:
helsinki.fi
Searching..
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>


# 1.6
docker build -t docker-clock .
docker run docker-clock

# 1.7
docker build -t curler .
docker run -it curler

# 1.8
docker run -v $(pwd) devopsdockeruh/first_volume_exercise

# 1.9
docker run -p 80:80 devopsdockeruh/ports_exercise

# 1.10
docker build -t frontend .
docker run -p 5000:5000 frontend

# 1.11
docker build -t backend .
docker run -v $(pwd):/usr/app/logs.txt -p 8000:8000 backend

# 1.12
docker build -t frontend .
docker run -p 5000:5000 frontend

docker build -t backend .
docker run -v $(pwd):/usr/app/logs.txt -p 8000:8000 backend

# 1.13
docker build -t spring .
docker run -p 8080:8080 spring

# 1.15
dockerhub repo: eetuh/dockertraining

# 1.16
https://eetuhdockerheroku.herokuapp.com/

# 1.17
My favourite programming environment contains node and npm on ubuntu.
https://cloud.docker.com/u/eetuh/repository/docker/eetuh/eetuhdockerheroku