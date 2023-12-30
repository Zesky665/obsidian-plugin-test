---
{"dg-publish":true,"permalink":"/contents/docker/push-dockerfile-to-dockerhub/","tags":["Docker","Docker-Compose"],"created":"2023-12-18T16:45:59.539+01:00","updated":"2023-12-18T16:46:38.968+01:00"}
---


## Step 1: Log in
`docker login`

## Step 2: Build image
Navigate to dockerfile repo then run. 
`docker build -t image_name .`

## Step 3: Tag Image
`docker tag image_name:latest username/image_name:tag`

## Step 4: Push Image
`docker push username/image_name:tag`