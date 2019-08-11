Terminal Reservation system

Flight Information System

config Folder
	-contains setup for MySQL database
database Folder
	-contains DB schema, function for variable initialization and data
node_modules Folder
	-contains node modules
public Folder
	-contains css styles and images
routes Folder
	-contains js files for injection from database to front end
	-home.js corresponds to home.ejs, Terminalone.js corresponds to terminalone.ejs and etc

views Folder
	partials folder
		-contains frontend hmtl ejs files

-contains app.js and server.js for console and server initialization
-contains package.json for dependencies

----------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------

Crew Management System ("terminal" Folder)

node_modules Folder
	-contains node modules

public Folder
	-contains images

routes Folder
	-contains js files for injection from database to front end
	-index.js corresponds to index.ejs, user.js corresponds to user.ejs

views Folder
	-contains app.js for server initialization
	-contains package-lock.json and package.json for dependencies
	-contains terminal.sql for DB initialization

----------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------
Nodejs Modules used in the process

	- express: handle routing
   	- express-fileupload: handle upload
   	- body-parser: parse request
   	- mysqlL: database module
   	- ejs: templating language
   	- req-flash: flash message
   	- nodemon: install globally to run, normally pre-installed
	- faker: generate fake data
	- jest: js testing
to install all of those, run: npm install express express-fileupload body-parser mysql ejs req-flash faker jest --save
----------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------
how to run

	Requirements:
		- All of the modules above installed
		- nodejs install and setup
		- xampp server install and setup
		- phpmyadmin, come with xampp
	Provided that all of the requirements have been satisfied, we can go ahead to running the program
		1/ in nodejs terminal, navigate to the parent folder of the project
		2/ in phpmyadmin, create database named "terminal",import "schema.sql", "data.sql" from main/database folder. 
		3/ navigate to the main folder by using "cd main" command in the terminal, then run with "nodemon app.js"
		4/ navigate to the terminal(sub) folder by using "cd terminal" command, then run with "nodemon app.js"
	Notes: the main interface run on port 5000, while crew interface run on 5001		
	