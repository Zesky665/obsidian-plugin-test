---
{"dg-publish":true,"permalink":"/contents/docker/save-container-snapshot/","tags":["Docker","Docker-Compose"],"created":"2023-12-18T16:47:14.755+01:00","updated":"2023-12-18T16:47:48.177+01:00"}
---


# 1.  Find docker container ID
Run the following command. 
`docker ps`

# 2. Create the snapshot
Run the following command.
`docker commit ID IMAGE_NAME:TAG`