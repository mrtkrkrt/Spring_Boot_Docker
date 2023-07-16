## Spring Boot and Docker

Before getting started spring boot and docker, let's look at how traditional deployments work?
* In manual approach for deployment follows steps to:
    * Setup Hardware
    * Setup OS
    * Install Software (Java, Python, Node)
    * Setup Application Dependencies
    * Install application
* If we examine the steps above, there are many dependencies and time-consuming processes.
* In the other hand, when developer implementing this steps, there is a high chance of making mistakes.

Docker provides us to simplify deployment process and once you have docker image, irrespective of what the docker image contains you run it the same way.
Docker image has everything you need to run your application such as operating system, JDK etc.

So what docker provides?
* Standaridized Application Packaging: Same packaging for all types of applications.
* Multi Platform Support
* Isolation: Even if you have multiple containers running o the same machine, each container isolated from the other containers.

Let's look at start docker command:
````shell
docker container run -d -p 8080:8080 myorg/myapp:0.0.1:RELEASE
````
* Image is a set of bytes
* Container is a running image
* myorg/myapp is repository name
* 0.0.1.RELEASE is a tag version
* -p hostPort:containerPort
* -d detached mode

### Summary
* Docker Image: A package representing specific version of your application
* Docker Registry: A place to store your docker images
* Docker Hub: A registry to host docker images
* Docker Repo: Like Github repo
* Docker Container: Runtime instance of a docker image
* DockerFile: File with instructions to create docker image
* ![image](https://github.com/mrtkrkrt/Spring_Boot_Docker/assets/55550212/8f01cb83-e85b-4a24-9ff6-a0299c5954de)

