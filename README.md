# GOAL
Containerized  a video streaming application

# NOTICE
The work documented in this repository is based on the training material provided by Ashley Davis with the book "Bootstrapping Microservices with Docker, Kubernetes, and Terraform: A Project-Based Guide". See the LICENSE for additional information.

# Chapter 04 Version Notes

Example number 3 from Chapter 4 of [Bootstrapping Microservices](http://bit.ly/2o0aDsP).

In Chapter 4 of Bootstrapping Microservices you learn to develop and test a microservices application using Docker-Compose.

You need Docker and Docker-Compose installed to run this.

Boot it up from the terminal using:

    docker-compose up --build

You must now load the database fixture ./db-fixture/videos.json into your database. You can do this using Robo 3T or mongoimport.

**IMPORTANT**: Once you have used docker-compose and before you try to use the browser to test your app,  you will need to use Study 3T - next version of Robo 3T - to do the following:
* Create a new database named video-streaming
* Create a new collection inside the new database named videos
* Import our videos.json in the newly created collection

Then point your browser at http://localhost:4002/video?id=5d9e690ad76fe06a3d7ae416

