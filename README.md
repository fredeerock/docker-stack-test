**Generate docker-stack.yml file:**  
- `docker-compose -f 1/docker-compose.yml -f 2/docker-compose.yml config > docker-stack.yml`

**Run Docker Stack:**  
- `docker stack deploy -c docker-stack.yml STACKNAME`

**If necessary, update DockerHub images:**  
*Docker stack needs images instead of Dockerfiles.*  
- `docker build . -t USERNAME/REPONAME:TAGNAME`  
- `docker push USERNAME/REPONAME`
