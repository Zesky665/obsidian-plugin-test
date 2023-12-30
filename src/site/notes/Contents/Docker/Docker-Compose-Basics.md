---
{"dg-publish":true,"permalink":"/contents/docker/docker-compose-basics/","tags":["Docker","Docker-Compose"],"created":"2023-12-16T21:56:46.740+01:00","updated":"2023-12-18T16:37:03.842+01:00"}
---

## 1. Create docker-compose file

Create a  `docker-compose.yml` file with the following contents: 

```
services: # list of containers 
	prefect_agent: # name of container
		image: "zharec/prefect_agent:latest" # image the container is based on
		env_file: # path to file with env values
			- .env
```

## 2. Run Docker-Compose file

Run Docker-Compose file by navigating to the directory where the file is and running the following command. 

`docker-compose up`

## 2. Stop Docker-Compose file

Stop Docker-Compose file by navigating to the directory where the file is and running the following command. 

`docker-compose down`

