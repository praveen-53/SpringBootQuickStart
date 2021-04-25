# SpringBootQuickStart
You will have all the Packages created based on the MVC Architecture and you can create your own Classes where they are Required.
Login and Register Apis are done in this QuickStart project, you can use them and feel free to modify them as your requirement.
You can test your Apis in the swagger, as i have embedded the swagger you can run the application as a springboot Application and go to
the URL http://localhost:8080/swagger-ui.html to test your Apis.

Database:
--------
* Firstly create schema named **quickstart** in postgres Db.
* create **users** table with primary key using below queries:
CREATE TABLE quickstart.users (
	user_id bigint NULL,
	firstname varchar NULL,
	lastname varchar NULL,
	email varchar NULL,
	"password" varchar NULL
);
ALTER TABLE quickstart.users ADD CONSTRAINT users_pk PRIMARY KEY (user_id);
* create a sequence named **sequence_id** in postgres Db.
Note: Change the credentials of postgresDb accordingly in application.properties.
Hosted this springboot application in heroku.
swagger-url: https://springbootquickstart.herokuapp.com/swagger-ui.html 

Finally, if you thing some other common code need to be added to this repository then don't wait make a pull request :)  
