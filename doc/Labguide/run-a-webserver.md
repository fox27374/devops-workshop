# Run a webserver
## Commands
| Command | Description |
| --- | --- |
| docker | image and container command line interface |
---

## Tasks
### 1. Change to the current lab directory
**`cd 03`**  

### 2. Start an nginx container called web and mount the web-content folder
**`docker run -d -p 80:80 -v $(pwd)/web-content/:/usr/share/nginx/html/ --name web nginx:alpine`**  

### 3. Check the website in your browser

### 4. List the running container
**`docker ps`**  

### 5. Stop the container
**`docker stop CONTAINER_ID`**  

### 6. Remove unused containers
**`docker container prune`**  