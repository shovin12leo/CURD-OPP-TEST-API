# CURD-OPP-TEST-API

#Folder Structure
![image](https://github.com/user-attachments/assets/ca8a6715-4384-4c2b-80b1-86268060aad3)


node-mongo-crud/
├── config/
│   └── db.js                 # MongoDB connection setup
├── controller/
│   └── UserController.js     # Controller logic for user operations
├── models/
│   └── User.js               # Mongoose schema for the User model
├── routes/
│   └── UserRoutes.js         # API routes for user-related operations
├── service/
│   └── UserService.js        # Business logic for user operations
├── utils/
│   └── ErrorHandler.js       # Custom error handling middleware
├── node_modules/             # Auto-generated folder for dependencies
├── app.js                    # Main entry point for the application
├── package.json              # Project metadata and dependencies
├── package-lock.json         # Lock file for dependencies


#Setup
1.Initialize the project:
npm init -y 

2.Install the necessary dependencies:
npm install body-parser express mongoose nodemon

3.Run the application:
node app.js

4. Start MongoDB using Compass.


# CRUD Testing Instructions (Using Thunder Client in VSCode or Postman):-
1.POST:-http://localhost:3000/users # inserting data.

Body(JSON)
{
    "name":"Shovin",
    "email":"abc@gmail.com", # add 5 more data
    "age":19
}

2.GET:-http://localhost:3000/users #viewing  all data.

3.GET:-http://localhost:3000/users/oject _id # <object_id> with the actual _id of the user obtained after inserting data.

4.PUT:-http://localhost:3000/users/oject _id 
Body(JSON)
{
    "name":"Shovin MD"
}

5.DELETE:-http://localhost:3000/users/oject _id 

