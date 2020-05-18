### Infomation

This repository contains docker-compose for running application https://github.com/hl-service/go-api with MongoDB.

### Requirements
- [Docker](https://www.docker.com/) with docker-compose

### Instruction
1. Build an image from source code: https://github.com/hl-service/go-api
2. Push image to some docker registry. For example, [Docker Hub](https://hub.docker.com).
3. Clone this repository.
4. Create enviroment file ```.env``` from ```.env.example``` with command ```cp .env.example .env``` on Linux/MacOS or ```copy .env.example .env``` on Windows.
5. Set for enviroment variable ```API_IMAGE_PATH``` path to image on registry.
6. Run containers with command: ```docker-compose up -d```
7. Check ran containers: ```docker ps``` or ```docker container ls```. You should have 2 containers: api and mongo.

Now you can open in browser: ```http://0.0.0.0:8080/```
