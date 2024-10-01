# 0x04. Files manager

This project is a summary of this back-end trimester: authentication, NodeJS, MongoDB, Redis, pagination and background processing.

The objective is to build a simple platform to upload and view files:

* User authentication via a token
* List all files
* Upload a new file
* Change permission of a file
* View a file
* Generate thumbnails for images
You will be guided step by step for building it, but you have some freedoms of implementation, split in more files etc… (utils folder will be your friend)

Of course, this kind of service already exists in the real life - it’s a learning purpose to assemble each piece and build a full product.
# Requirements
Read or watch:
* Node JS getting started
* Process API doc
* Express getting started
* Mocha documentation
* Nodemon documentation
* MongoDB
* Bull
* Image thumbnail
* Mime-Types
* Redis

# Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

* how to create an API with Express
* how to authenticate a user
* how to store data in MongoDB
* how to store temporary data in Redis
* how to setup and use a background worker

## Tasks :

#### 0. Redis utils
Inside the folder utils, create a file redis.js that contains the class RedisClient.
    
#### 1. MongoDB utils
Inside the folder utils, create a file db.js that contains the class DBClient.
    
#### 2. First API
Inside server.js, create the Express server:

* it should listen on the port set by the environment variable PORT or by default 5000
* it should load all routes from the file routes/index.js
    
#### 3. Create a new user
SNow that we have a simple API, it’s time to add users to our database.
    
#### 4. Authenticate a user
In the file routes/index.js, add 3 new endpoints:

* GET /connect => AuthController.getConnect
* GET /disconnect => AuthController.getDisconnect
* GET /users/me => UserController.getMe
    
#### 5. First file
In the file routes/index.js, add a new endpoint:

* POST /files => FilesController.postUpload
Inside controllers, add a file FilesController.js that contains the new endpoint:
    
#### 6. Get and list file
   
#### 7. File publish/unpublish
    
#### 8. File data
    
#### 9. Image Thumbnails