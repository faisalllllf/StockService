The Spring boot service will provide near real-time stock quotes to client applications.

In this document I will provide the details of spring boot service and how to run that application.

1.)	  Source code for the Spring Boot backend service.
  You can clone this project from my GitHub repo or download the   
   attached zip file which I have shared.
  url: https://github.com/faisalllllf/StockService.git


2.)	Api Documentation :
I have attached the list of Api’s I have created you can import the Json file in postman and access those Api’s.
Those Api’s also you can find in this
     url: https://github.com/faisalllllf/StockService.git

3.)	Instructions on how to run the service.
You can directly run the service from Eclipse or spring tool Suite by 
Importing attached zip file 
Or 
After importing zip file you can run docker create docker image for docker file I have created in project and run the docker image.

 For creating docker image 
 docker build -t RealTimeApp .

 for Run that image after it is created 
 docker run -p 8080:8080 RealTimeApp.

 IMPORTANT Note:
 Need to create a database in your local mysql so that you can first    register into Real time application.

Steps:
1.)	First create database in your MySQL local
2.)	As Iam using JPA implementation so if you create database name is enough no need to create tables in your local
3.)	Invoked Register Api first register yourself
4.)	Then invoke login Api you will get a jwt token.
5.)	Then for stock Get and Get All Api’s use that Authorization token as Header and invoke the Api.
 



