# Coding test for United Remote
#### Arash Tajdar

## About the project

- Sanctum for Auth
- Laravel collections to display the result in better way
- Faker and factory for feature tests
- feature tests can be extended, but I think that is enough for now. let me know if you want me to extend it and write more deep tests.
- I wrote some annotations to document my lines, also I wrote some comment for documentations. I think those are enough because the other parts of my code are clearly readable, but this one also can be extended :)
- I added category table, and it's relation to product table just to show how I use relations in migration file and in models and controllers. I can also extend it and create new tables.
- Docker implemented. It was better and easier to use sail, but I prefer to create the Dockerfile by myself.
- Docker and related files need many improvements (needs some more time), but it is good for now.

## How to run the project

1. Create .env file and Copy .env.example file to this new file
2. Change variable like this
   ``
   DB_CONNECTION=mysql
   DB_HOST=db
   DB_PORT=3306
   DB_DATABASE=laravel
   DB_USERNAME=laravelUser
   DB_PASSWORD=@wn12341818
   ``
   - It is important to : 
     - change host variable to db 
     - set a new username and password 
     - change the name of the database to laravel (you can modify this in docker-compose/mysql/db_init.sql file) 
       
Or you may encounter errors on running db-container

3. Run ./init.sh bash file or alternatively run all the commands in this file one by one (* it may take a long time to generate autoload file*)
4. Run localhost:8000 and use Postman collection (United Remote.postman_collection.json) in root folder to send requests

