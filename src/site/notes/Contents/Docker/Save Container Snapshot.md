---
{"dg-publish":true,"permalink":"/contents/docker/save-container-snapshot/","tags":["Docker","Docker-Compose"],"created":"2024-02-29T00:08:23.435+01:00","updated":"2024-02-29T00:08:23.436+01:00"}
---


# 1.  Find docker container ID
Run the following command. 
`docker ps`

# 2. Create the snapshot
Run the following command.
`docker commit ID IMAGE_NAME:TAG`