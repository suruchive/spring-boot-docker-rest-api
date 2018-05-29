# spring-boot-docker-rest-api
Building RESTFul API Services using spring boot and MySQL with containerization using Docker

Steps for executing :

1. Clone/Download the repository.

2. Open the project in the IDE (Netbeans/Intellij Idea/Eclipse) and generate the executable .jar file for the application. The alternate method to generate the .jar file is through Maven.
   
3. Rename **docker-compose-sample.yml** file to **docker-compose.yml**.

4. Open **docker-compose.yml** file and add the MySQL (db) environment parameter values and Spring REST API (spring-rest-api) environment parameter values for database connection from the the application.

5. Open the terminal and go to the directory where docker-compose.yml is located and run the below command in -d (Detach Mode) and will build the MySQL and Spring Boot Rest API Containers.

   		docker-compose up -d

6. Run the below command to get the list of running containers :

		  docker ps
    
7. After executing above steps without any errors and docker containers are up and running, open the browser and navigate to below url:
    
		  http://localhost:9090/swagger-ui.html#/
      
