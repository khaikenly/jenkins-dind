# Jenkins with Docker in Docker

- "This Docker Compose file runs Docker-in-Docker (DinD) and Jenkins containers. You can build Docker images in a Jenkins pipeline."

### Run with Docker
```
docker-compose up -d --build
```

### Access to Jenkins
```
localhost:8080
```

### Initial Admin Password
- Exec to container 'jenkins'
```
docker exec -it jenkins bash
cat /var/jenkins_home/secrets/initialAdminPassword
```