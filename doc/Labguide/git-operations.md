# Git Operations
## Commands
| Command | Description |
| --- | --- |
| git |  |
| docker compose | docker but declarative |
| nano | modify textbased files |
| ls | list files |
---

## Tasks
### 1. Change to the current lab directory
**`cd LAB_NUMBER`**  

### 2. Clone the workshhop git repo
**`git clone https://github.com/fox27374/devops-workshop-repo.git`**  

### 3. Change to the newly created directory
**`cd devops-workshop-repo`**  

### 4. List the files in the directory
**`ls -la`**  

### 5. Build the docker image
**`docker build -t splunk:workshop .`**  

### 6. Start the container and check is its running
**`docker compose up -d`**  
**`docker ps`**  

### 7. Find the problem  - Hint: Check the variables in the compose file
**`docker logs -f CONTAINER_NAME`**  
**`nano compose.yml`**  

### 8. Add an .env file and add the missing variable
**`nano .env`**  

### 9. Start the container again and check is its running
**`docker compose up -d`**  

