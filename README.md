1. Create and push any needed Docker images to DockerHub

2. Initiate Docker Swarm
- `docker swarm init`

3. Generate docker-stack.yml file:
- `docker-compose -f 1/docker-compose.yml -f 2/docker-compose.yml config > docker-stack.yml`

4. Run Docker Stack:
- `docker stack deploy -c docker-stack.yml STACKNAME`