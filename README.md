# Django_Docker-Compose_Postgress data application
This project is created as part of technical assignment. Purpose: Purpose of this project is to create a Django web server application and connect it to postgres database in backend. Both applications must be inside the Docker environment and containerized using docker-compose. This has been achieved. Windows environments have been used to install the docker application.
Procedure:
   1. Installed the docker compose application.
   2. Created a project directory called DJANGO.
   3. Under the project directory, Dockerfile will install the python image which can be run as a container once built.
   4. Create a requirement.txt file. This file will be called in Dockerfile and will install Django and Postgres applications accordingly.
   5. Create docker-compose.yaml file. We are creating a web server application which is dependent on postgres database service.
   6. Now we have all the files ready.
   7. We will use docker-compose to create the environment. 
         command: docker-compose run django django-admin startproject core . ### This will build the Django application and progress in containers.
   8. use the "docker-compose up" command to start the web app.
   9. Diff command can be used: 
         "docker-compose down" - to stop the containers 
         "docker exec -it django bash"- to get into web app terminal 
         "docker exec -it pgdb psql -U postgres" - to login to postgres database 
         "\c" - to connect database 
         "\d" - list all the records 
         "\q" - exit the database

          
  
