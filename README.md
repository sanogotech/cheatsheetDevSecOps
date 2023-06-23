## References of Devops



## Docs

- https://medium.com/@adewopol/devops-project-8ef09a0e172a

## DevSecOps  REX

![DevSecoPS REX AWS](https://github.com/sanogotech/cheatsheetDevSecOps/blob/master/docs/CICDJenkinsSonarqube.jpg)

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

