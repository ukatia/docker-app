# docker-app
A sustainable web application that can be easily deployed and maintained using Docker

### File Structure
```
docker-app/
   /traefik: Traefik Load Balancer - Configuration
   /node-app: Nodejs app with Postgresdb
```
``` 
Update the applications containers without an interruption of service:
docker-compose up -d --build
This will rebuild all images defined in your compose file, then restart any containers whose images have changed.
```
```
docker-compose.yml:
- Contains three services for the three containers.
- Create network "traefik-global-proxy" when running "docker-compose up"
- NodeJs app creates the db
