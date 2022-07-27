# Azure Training - Docker

## Case

Developers have created a <b>NodeJS</b> application for products microservices. As DevOps engineer you are supposed to containerise the NodeJS application. The NodeJS version used is <b>v16.3.4</b>.

We need to create a docker image for the <b>development environment</b>, where developers also need <b>Nodemon</b> (a nodejs development tool). This tool need to be installed at the global level in container.

The application runs on port 3001, with index.js as entry file for the application.

We will need a mysql container for the application to run. Generate a connection string and add it in the .env.dev file.

The mysql container will have a database named "products" which will be access by user "john" with password "John123" with full privileges only on that database.

The application and container should be in a network where they can resolve their dns names.

## Docker commands we will be using

 - docker run
 - docker start
 - docker stop
 - docker rm
 - docker network
 - docker volume
 - docker logs
 - docker exec