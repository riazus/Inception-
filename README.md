# Inception
Introduction to docker technology with own web-site 

Commands for evaluation:

1. redis checking
   docker exec -it redis redis-cli monitor

2. adminer
   http://localhost:8080/

3. portainer
   1. docker volume create portainer_data
   2. docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest
