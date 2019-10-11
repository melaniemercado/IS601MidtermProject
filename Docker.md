# Docker Tutorial

**What is Docker?**
Docker is a platform for developers and sysadmins to **build, share, and run** applications with containers. The use of containers to deploy applications is called _containerization_. Containers are not new, but their use for easily deploying applications is.

Containerization is increasingly popular because containers are:

-   Flexible: Even the most complex applications can be containerized.
-   Lightweight: Containers leverage and share the host kernel, making them much more efficient in terms of system resources than virtual machines.
-   Portable: You can build locally, deploy to the cloud, and run anywhere.
-   Loosely coupled: Containers are highly self sufficient and encapsulated, allowing you to replace or upgrade one without disrupting others.
-   Scalable: You can increase and automatically distribute container replicas across a datacenter.
-   Secure: Containers apply aggressive constraints and isolations to processes without any configuration required on the part of the user.

# Build and test your image:

1) Now that we have some source code and a Dockerfile, it’s time to build our first image, and make sure the containers launched from it work as expected. 

![enter image description here](https://lh3.googleusercontent.com/k36o2YMI2ebtjGN6LXt5BCvYcPcxnsOMsEZN1Di9TJy7JIuH6-Itz1q4PpCYd9-s3-c2jGb2AFY)

Make sure you’re in the directory `node-bulletin-board/bulletin-board-app` in a terminal or powershell, and build your bulletin board image:

2) Start a container based on your new image:

![](https://lh3.googleusercontent.com/gEBre1L5BQLgCnTD3L8iLk9s9w38gR_PJGuMsFOGEdVuAdEiY_xSQewOcZU4oEFnaqGBBTLMpcU)

 We used a couple of common flags here:  `--publish`  asks Docker to forward traffic incoming on the host’s port 8000, to the container’s port 8080 (containers have their own private set of ports, so if we want to reach one from the network, we have to forward traffic to it in this way; otherwise, firewall rules will prevent all network traffic from reaching your container, as a default security posture).  `--detach`  asks Docker to run this container in the background. `--name`  lets us specify a name with which we can refer to our container in subsequent commands, in this case  `bb`. Also notice, we didn’t specify what process we wanted our container to run. We didn’t have to, since we used the  `CMD`  directive when building our Dockerfile; thanks to this, Docker knows to automatically run the process  `npm start`  inside our container when it starts up.
 
 3. Visit your application in a browser at  `localhost:8000`. You should see your bulletin board application up and running. At this step, we would normally do everything we could to ensure our container works the way we expected; now would be the time to run unit tests, for example.

4. Once you’re satisfied that your bulletin board container works correctly, delete it:

![](https://lh3.googleusercontent.com/PIoxo4YKFRu_6iQDn1gyCF5WxzV6eYiBuWFHnE5Q6l2CXO_LCe8CgzTJ0DdKipVbRzoGevhBgDY)
