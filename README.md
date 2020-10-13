# REST-API-using-Python

To develop an API interface for MongoDB and deploy our program to Docker.
---
### First Things First 
1. Install Docker
2. Install MongoDBCompass Community
3. Install Postman

## 1. How to deploy the docker container.
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
## 2. How to access APIs on localhost.
## 3. How to use these APIs to list, add, delete or update products.
