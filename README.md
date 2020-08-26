# Docker workshop

## How to run
Go to folder `dashboard`.

To run using **docker compose**:
### 1. Build the image
`docker-compose build`

### 2. Run the services
`docker-compose up`

### 3. View dasboards
* Go to `http://0.0.0.0:8080` (or `http://localhost:8080`) to view barplot app.
* Go to `http://0.0.0.0:8050` (or `http://localhost:8050`) to view histogram app.

### 4. Shut down the services
* Stop the apps: `docker-compose shut`
* Stop the apps and delete the containers: `docker-compose down`

## Other useful commands
* Check for running containers: `docker ps`
* List all containers: `docker ps -a`
* List docker images: `docker image ls`
* Delete an image: `docker image rm $image_name`
* Delete a container `docker container rm $container_id`
* Build an image without docker compose: `docker build -t $image_name .`
* Run a container without docker compose: `docker run $image_name`
