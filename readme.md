
# Installation
## Build the Jenkins BlueOcean Docker Image
```
## Create the network 'jenkins'
```
docker network create jenkins
```

##  launch Containers
docker-compose up -d


## Get the Password
```
docker exec jenkins1 cat /var/jenkins_home/secrets/initialAdminPassword
```

## Connect to the Jenkins
```
https://localhost:8081/
```

## Installation Reference:
https://www.jenkins.io/doc/book/installing/docker/


## alpine/socat container to forward traffic from Jenkins to Docker Desktop on Host Machine

https://stackoverflow.com/questions/47709208/how-to-find-docker-host-uri-to-be-used-in-jenkins-docker-plugin

## to get Ip address to user with docker agent setup in Jenkins
```
docker inspect agent3 | grep IPAddress

