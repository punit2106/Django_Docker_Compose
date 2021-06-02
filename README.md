# Django_Docker-Compose_Postgress data application
This project is created as part of technical assignment. 
Purpose: Purpose of this project is to create a Django web server application and connect it to postgres database in backend. Both application must be inside within Docker environment and containarized using docker-compose. This has been achieved. Windowds enviroment have been used to installed the docker application.

Procedure:
   1.  Installed the docker compose application.
   2.  Created a project directory called DJANGO.
   3.  Under project directory, Dockerfile will install the python image which can be run container once built.
   4.  Create requirement.txt file. this file will be called in Dockerfile and will installed Django and Postgres application accordingly.
   5.  Create docker-compose.yaml file. We are creating a web server application which is dependent on postgres database service.
   6.  Now we have all the files ready.
   7.  We will use docker-compose to create the enviroment.
       command: docker-compose run django django-admin startproject core .  ### this will build the Django application and progress in containers. 
   8.  use "docker-compose up" command to start the web app.
   9.  Diff command can be used: 
          "docker-compose down" - to stop the containers
          "docker exec -it django bash"- to get into web app terminal
          "docker exec -it pgdb psql -U postgres" - to login to postgres database
          "\c" - to connect database
          "\d" - list all the records
          "\q" - exit the database
          
  
