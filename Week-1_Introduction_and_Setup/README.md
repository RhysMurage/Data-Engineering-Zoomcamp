# Introduction and Setup

## Technologies
### Docker
![Alt](Images/docker-logo.png)
> This is a containerization platform that enables the delivery of software in packages called containers

> Some of the commands learnt are:
1. **docker run -it python:3.9**
    > creates an image in a container with python:3.9 as the base image

2. **docker run --help**
3. **docker run -it --entrypoint=bash python:3.9**
    > __entrypoint=bash__ : will install bash and run it at the **start** rather than the **python prompt**

4. **docker build -t test:pandas .**
    > _test:pandas_ : name(test) and version(pandas) of the image created

    > **_._** : tells docker to install the **Dockerfile** in the current directory 

> We use docker to run data pipelines in an isolated environment. Data piplines are processes and services that take in data and outputs more data

> **Dockerfile** contains the instructions of what packages to run when creating a new image in the container. It contains the following:
- FROM [baseimage]
- RUN pip install <package> : packages to be installed
- WORKDIR : creates a directory where pipeline will be located
- COPY <**source**> <**destination**> : copies files from destination located in the same directory to a new file that will be in the container
- ENTREPOINT : tells what docker to do run when the image is created.