# Introduction and Setup

## Technologies
### Docker
![Alt](Images/docker-logo.png)
> This is a containerization platform that enables the delivery of software in packages called containers

> Some of the commands learnt are:
1. **docker run -it python:3.9**
2. **docker run --help**
3. **docker run -it --entrypoint=bash python:3.9**
4. **docker build -t test:pandas .**
    > _test_ : name of the image created

    > **_._** : tells docker to install the **Dockerfile** in the current directory 

> We use docker to run data pipelines in an isolated environment. Data piplines are processes and services that take in data and outputs more data

> **Dockerfile** contains the instructions of what packages to run when creating a new image in the container