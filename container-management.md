# Container management
### General Commands
- - podman container list –all

### Running Containers
- podman run -d -p 8080:80 --name nginxtest  nginx:latest

- **Remove Container**
	- podman rm "containerid" 
- **Remove Image**
	- podman image rm "imageid"    
- podman stats 
- podman diff