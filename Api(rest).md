# About Api and it's development

Api :
Application Programming Interface

this is a frontend/program that can be used to interact with other application that some other developer wrote and can access their resources without actually being aware of the underlying code/architecture

Ex: Twitter api(you can access the tweets and post tweets to the site without actually explicitly using their app/site , the user can then build a app/site that performs specific task with this api), can post comments to posts, take user details with google after a single sign on with google etc.
travel booking sites are best example they interact with multiple travel services databases api’s and use their output to aggregate the result the user might ask for in real time




RestFul API:
Since an api is a medium between the actual application/service and the user application it can be used in only specific places with specific functionalities 

categories of api’s are :
gaming api’s , ui api’s , web api’s etc

Rest is a web api, which is a alternative for RPC & SOAP api standards

Rest is more of technology and standard then a software, it is in popularity due to it’s better view on use of api on web for different purposes:


Rest is used mostly with http

http has over 39 methods(verbs called in general slang)/these are functions that does a particular job specified 


most used http methods are
GET	: gets data of specific resource
POST 	: sends specific resource to the end point
PUT	: overwrites a specific resource
DELETE: deletes a specific resource
HEAD	: gets the head of the data of a specific resource(just like get)


every time we access a url we are indeed using a get method associated with http.

to test and learn of api’s of different services/application use apigee.com


every website and application can have their own internal method using http verbs/methods

so we can search for a resource of a service with get method and use their specific method like photos.search in the url itself 


some api’s need authentication to verify the user and block if necessary




Creating a api:

create an app 
then install rest
pip install djangorestframework

and add both  to settings
‘rest_framework’
‘applicationname’

goto models of application 


import psycopg2
connection = psycopg2.connect(user="postgres", password="accession", host="127.0.0.1", port="5433", database="doc")
cursor = connection.cursor()
q = "CREATE TABLE ROOM(ROOM INT PRIMARY KEY NOT NULL, URL CHAR(50) NOT NULL)"
cursor.execute(q)
connection.commit()
cursor.close()
connection.close()
