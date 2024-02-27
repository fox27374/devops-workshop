# Connecto containers
## Commands
| Command | Description |
| --- | --- |
| docker | image and container command line interface |
---

## Tasks
### 1. Change to the current lab directory
**`cd LAB_NUMBER`**  

### 2. Create a new docker network
**`docker network create grafana`**  

### 3. Start the prometheus container
**`docker run -d --rm -v $(pwd)/prometheus.yml:/etc/prometheus/prometheus.yml -v prom_data:/prometheus --net grafana --add-host host.docker.internal=host-gateway --name prometheus prom/prometheus`**  

### 4. Start the grafana container
**`docker run -d --rm -p 80:3000 -v $(pwd)/datasource.yml:/etc/grafana/provisioning/datasources/datasource.yml -e GF_SECURITY_ADMIN_USER=admin -e GF_SECURITY_ADMIN_PASSWORD=grafana --net grafana --name grafana grafana/grafana`**  

### 4. Check the website in your browser

### 5. Display one metrics graph
* Menu
* Explore
* Select **`prometheus_http_requests_total`**

### 5. Stop the container
**`docker stop grafana`**  
**`docker stop prometheus`**  
