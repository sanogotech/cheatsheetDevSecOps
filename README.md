## References of Devops



## Docs

- https://medium.com/@adewopol/devops-project-8ef09a0e172a


## How to connect to the Docker host from inside a Docker container?

* https://github.com/sanogotech/connect-docker-host-from-docker-container-example

* https://github.com/sanogotech/wordpress-docker-compose


```
  services:
  wp:
    image: wordpress:latest # https://hub.docker.com/_/wordpress/
    ports:
      - ${IP}:${PORT}:80 # change ip if required
    volumes:
      - ./config/php.conf.ini:/usr/local/etc/php/conf.d/conf.ini
      - ./wp-app:/var/www/html # Full wordpress project
      #- ./plugin-name/trunk/:/var/www/html/wp-content/plugins/plugin-name # Plugin development
      #- ./theme-name/trunk/:/var/www/html/wp-content/themes/theme-name # Theme development
    environment:
      WORDPRESS_DB_HOST: db
      WORDPRESS_DB_NAME: "${DB_NAME}"
      WORDPRESS_DB_USER: root
      WORDPRESS_DB_PASSWORD: "${DB_ROOT_PASSWORD}"
    depends_on:
      - db
    links:
      - db
  
```

## DevSecOps  REX

![DevSecoPS REX AWS](https://github.com/sanogotech/cheatsheetDevSecOps/blob/master/docs/CICDJenkinsSonarqube.jpg)

##  Flow  DevOps

![Flow  DevOPS ](https://github.com/sanogotech/cheatsheetDevSecOps/blob/master/docs/CIFlow.jpg)

## Build and push a container image to Docker Hub from your computer

![Docker Image Container ](https://github.com/sanogotech/cheatsheetDevSecOps/blob/master/docs/dockerFileImageContainer.jpg)

Start by creating a Dockerfile to specify your application as shown below:

*  Code Sample :

    - https://github.com/sanogotech/docker-sample-nginx
 
   

```
# syntax=docker/dockerfile:1
FROM busybox
CMD echo "Hello world! This is my first Docker image."

```


Run 

```
docker build -t <your_username>/my-private-repo .
```

 to build your Docker image.

Run 
```
docker run <your_username>/my-private-repo 
```

to test your Docker image locally.

Run 
```
docker push <your_username>/my-private-repo 
```

to push your Docker image to Docker Hub. You should see output similar to:

Run 
```
docker exec -it container-name sh
```

```
docker logs <contaner> > <logfile.txt>
```

