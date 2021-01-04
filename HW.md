# reverse-engineering

##
Reverse engineering code HW

Starting with the config file, located inside is a folder called “middleware” containing isAuthenticated.js. This file prevents further access and will redirect them to the login page. 
Also included is a configuration(“config.json”) to the server and a passport.js file which shows the passport call to login with the users email and password. 

Next, the models folder includes an index.js and user.js files. The index.js connects the user to the database and imports the user's login information. User.js shows the user model where bcrypt is called for password hashing. This secures the database.

Next are node-modules which are dependencies installed using npm install.

In the routes folder, is api-routes and html-routes. Both of these files contain routes for the user to sign in. The api-routes specifically grabs necessary data to display onto the client side. The html-routes file checks if the user is logged in and redirects them to the correct page.

Package.json contains all info, modules used, versions and many other key information.

Server.js creates the server port which requires all necessary packages and configures middleware for authentication and syncs all data to the database. 
