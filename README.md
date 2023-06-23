## References of Devops

<<<<<<< HEAD


## Build and push a container image to Docker Hub from your computer

Start by creating a Dockerfile to specify your application as shown below:

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


docker exec -it container-name sh

docker logs <contaner> > <logfile.txt>
=======
## Docs

- https://medium.com/@adewopol/devops-project-8ef09a0e172a
  
## DevSecOps  REX

![DevSecoPS REX AWS](https://github.com/sanogotech/cheatsheetDevSecOps/blob/master/docs/CICDJenkinsSonarqube.jpg)
>>>>>>> 208b0e4b2f1ea2ed85d55cf36c780ed6ad62f093
