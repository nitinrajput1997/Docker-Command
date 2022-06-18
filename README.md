# Docker-Command

#### Run
```bash
docker run
```

To run the container

#### PS
```bash
docker ps 
docker ps -a 
```

To list the running container

#### Stop
```bash
docker stop container_name
```

To stop the running container

#### RM
```bash
docker rm container_name
```

To stop and remove the container permanently


#### Images
```bash
docker images
```

To get the list of images

#### RMI
```bash
docker rmi image_name
```

To delete/remove the images

#### Pull
```bash
docker pull image_name
```

To pull/download the docker images but does not run it

#### Append Command
```bash
docker run ubuntu sleep 10
```

It will exit after sleeping 10s otherwise it will exit instantly because no process was running to make container running

#### Naming Container
```bash
docker run -d --name nitin_container image_Name
```

This will assign name to a container when it runs

#### Port Mapping
```bash
docker run -p 80:5000 nitinrajput/app
```

#### Volume Mapping
```bash
docker run -v /opt/datadir:/var/lib/mysql mysql
```

Whenever the container runs, it will stores the data to external volume directory. Due to which, if somehow container remove then the data will remain in external directory

#### Inspect
```bash
docker inspect container_name or _ID 
```

To see the detailed information about the container

#### Logs
```bash
docker logs container_name or _ID
```

To see the logs of conatiner
