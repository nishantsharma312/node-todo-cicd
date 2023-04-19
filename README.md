# Jenkins Project Deployment

## Table of Contents
* [Prerequisites](#prerequisites)
* [Jenkins](#jenkins)
* [Webhook](#webhook)
* [Build-steps](#build-steps)

## Prerequisites

  1. AWS EC2 instance/Linux installed
  2. Java Installed
  3. Jenkins Installed
  4. Docker Installed
  5. Docker-compose Installed
  6. sudo permissions given to Jenkins(sudo usermod -a -G docker Jenkins)
  7. Create Dockerfile and docker-compose.yml file for the application.

## Jenkins

  1. Create a new item and choose a free-style project.
  2. In the General setting provide the project description.
  3. Now, go to Source code management to configure GitHub to Jenkins. Provide the GitHub URL where the code exists. 
   
## Webhook
  
 - Configure GitHub Webhooks in repository settings.Choose just push event option.

## Build-steps
  
 - Now, go to Jenkins and navigate to the build steps of the project. Provide the docker-compose commands.
________________________________

$ docker-compose down

$ docker-compose up -d --no-deps --build web
________________________________
 - Now,build the project and check if the build is successfully completed. Finally open port 8000.
 - Now if any change is committed in our repository our project will be automatically updated.


## Contact

- Connect with me on LinkedIn [Nishant Sharma](https://www.linkedin.com/in/nishant-sharma-03012000)
- Twitter [Nishant Sharma](https://twitter.com/_Nishant312)
- Project Link [node-todo-cicd](https://github.com/nishantsharma312/node-todo-cicd)

