# Docker compose basic
## 
| Command | Description |
| --- | --- |
| docker compose | change directory |
| nano | modify textbased files |
| ls | list files |
---

## Tasks
### 1. Change to the lab directory
**`cd lab`**  

### 2. Edit the compose.yml file
**`nano compose.yml`**  

### 3. Change the port mapping to the correct host port

### 4. Start the container using docker compose
**`docker compose up -d`**  

### 5. Check if you can see the nginx default page in your browser

### 6. Stop the container
**`docker compose down`**  

### 7. Add a volume to mount the index.html file into the container
**`./index.html:/usr/share/nginx/html/index.html`**  

### 8. Start the container
**`docker compose up -d`**  

### 9. Check if you can see the changed index page

### 10. Stop the container
**`docker compose down`**  

### 11. Add a secont container
**`docker compose down`**  