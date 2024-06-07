---
{"dg-publish":true,"permalink":"/contents/docker/running-scripts-in-docker/","tags":["Docker","Docker-Compose","Scripts"],"created":"2024-06-07T17:41:41.644+02:00","updated":"2024-06-07T17:41:41.644+02:00"}
---


## 1. Create script

`touch script.sh`
`echo "#!/bin/bash" >> script.sh` - otherwise you're going to get a format error. 
`echo "YOUR_BASH_CODE" >> script`
`chmod +x script.sh` - to make it executable

## 2. Add it to a dockerfile

In the dockerfile add: 

`COPY script.sh`
`RUN chmod +x docker_setup.sh`
`RUN ./docker_setup.sh`

## 3. Run the script

Add:
`ENTRYPOINT or COMMAND` to dockerfile. 

OR 

`entrypoint: or command:` to docker-compose.

### 4. Run in a running container

Run inside of a running container using `exec`

`docker exec -it container_name ./docker_setup.sh