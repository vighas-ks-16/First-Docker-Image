# First-Docker-Image
My First Docker Image 


🐳 Just embarked on a Docker journey! 🚀

Setting up Docker on an EC2 instance and getting acquainted with its basics has been a fantastic learning curve.

Here's a glimpse of what I've learned so far:

To install Docker on an EC2 instance, use the command :

```
sudo apt install docker.io -y
```

To verify whether Docker is Running or not, use the command :

```
sudo systemctl status docker
```

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/88bc0442-f47b-4256-be91-94bc897990a3)


To verify whether Docker is Ready to use or not, use the command :

```
docker run hello-world
```

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/9e214073-a1d8-4acc-bc10-daf4933634f2)


To add ubuntu user to the Docker group, use the command :

```
sudo usermod -aG docker ubuntu
```

Restart the session for the changes to be reflected :

```
logout
```

```
docker run hello-world
```



### First Docker File 

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/415fd294-41e7-49e3-8be9-32e9ca9a6310)


Building the Docker Image in my DockerHub :

```
docker build -t vighasks/my-first-docker-image:latest .
```

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/400d232e-2435-4975-b455-c43b020d3de8)

Utilized the 'docker build' command to transform Dockerfiles into Docker images, a process facilitated by the Docker daemon.



To create a Docker Container based on the specified Docker Image, use the command :

```
docker run -it vighasks/my-first-docker-image:latest
```

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/13389382-d80a-4db8-8a34-dc9bf5f5ecbe)

Witnessed the magic of 'docker run' command, which materializes Docker containers from Docker images, encapsulating system dependencies and application components.


Login with your Docker Credentials to push or pull images from the DockerHub

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/8d36020e-ac5f-4a4a-a5d9-6ba63ecd1549)



To push the Container Images to the DockerHub (Global Registry for Docker Images), use the command :

```
docker push vighasks/my-first-docker-image:latest
```

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/04b6d12e-38bd-46a5-bfef-223751bb1895)

To pull your Container Images from the DockerHub, use the command :

```
docker pull vighasks/my-first-docker-image:latest
```

To list all the locally available Docker Images on the system, use the command :

```
docker images
```

### Final Outcome of the Project in the DockerHub :

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/8cb8d7a3-6e4d-49c8-a330-17fb9a3ac0d9)

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/ddc301ad-6892-45af-b78e-28c3ded19b14)

![image](https://github.com/vighas-ks-16/First-Docker-Image/assets/107311113/78bdcab4-88b1-439e-9a53-2c4be18b4c63)






### Conclusion :


We have explored the Docker lifecycle, understanding how Docker client communicates with the Docker daemon, which, in turn, listens to Docker API requests.


Docker Hub emerged as a go-to platform, serving as a version control system for Docker images, ensuring seamless collaboration and distribution.

