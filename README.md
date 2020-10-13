# REST-API-using-Python

To develop an API interface for MongoDB and deploy our program to Docker.
---
### First Things First 
1. Install Docker
2. Install MongoDBCompass Community
3. Install Postman

### Getting Started with docker and mongodb

Step 1: Setting up Docker
-------------------------
Before anything we need to install latest version of Docker. Type in the following command in Command Prompt to check the version of the docker install on your system
```bash
docker -v
```

Step 2: Pulling MongoDB Image
-----------------------------
An image consists of all the necessary files required for setting up an application or multiple copies of this application in the form of containers.
```bash 
docker pull mongo
```

Step 3: Creating a container for MongoDB
----------------------------------------
To run the image, we need to create a container for the MongoDB on Docker. Following code will help us to do so.
```bash
docker create -it --name MongoContainerName -p 5000:27017 mongo
```
To start and stop the container in use we can use following commands. 
Run this command to start it
```bash 
docker start MongoContainerName
```
To stop a container we use
```bash
docker stop MongoContainerName
```

Step 4: Creating MongoDB Interactor
-----------------------------------
In this step, we will be creating API using Flask and pymongo.

 1. First, install and import libraries like Flask and pymongo
 2. Create MongoDB interactor
 3. Creating a Flask Server
 4. Defining CRUD HTTP Methods.
 
Step 5: Deploying our code on Docker
------------------------------------
Within this particular step, we will get to know on how to deploy code on Docker and how to link 2 Docker containers internally.
 1. Dockerfile is a configuration file for our program. It defines the basic working environment for our application and also defines how our applications are going to interact with external environments.

 2. After creating our Dockerfile, we need to create a docker-compose file. A Docker-Compose file allows us to link multiple containers and run them at the same time.
      
Time to run the containers-
```bash
docker-compose run --build    
```

## 1. How to deploy the docker container.
## 2. How to access APIs on localhost.
In order to access APIs on localhost, we will use Postman. It is a great tool when trying to dissect RESTful APIs made by others or test ones you have made yourself. It offers a sleek user interface with which to make HTML requests, without the hassle of writing a bunch of code just to test an API's functionality.
![banner_postman](https://mms.businesswire.com/media/20200206005191/en/728482/22/pm-logo-vert.jpg)
## 3. How to use these APIs to list, add, delete or update products.
