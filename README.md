**INTRODUCTION**

Built a bookstore management system using GoLang, CRUD API’s integrated with  MySQL Database, we’ll be using the gorm package to interact with our database. We used JSON marshalling to convert the database into json file and gorilla for routing . 
The project diagram are there for further clear explanations


**ABOUT PROJECT FILES**
We have two main folders -
- 1. ***Cmd folder*** - we have main.go file
- 2. ***Package folder*** - we have 5 folders inside this i.e. config, controllers, book models, routes, and utils folder.
- Inside config folder we have app.go file which helps us to connect with the database.
- In controllers we have the functions that helps us to process the data that we’ll get for as response and the requests that we’ll get from the user and the response that we need to send to the user. Later we’ll process all this in book controller.
- In book controller we have book.go file which helps us to create those structs and models that will be used by our database.
- In routes helps in getting the controller files and methods for a request by the user.
- In utils we have some code for marshalling and marshalling json from our response and a request.


**GETTING STARTED**

*STAGE -I*
- Open the terminal 
- Make the directory where you will store all the files, for that use command $mk go-bookstore(project name)
- Jump in the project file $cd go-bookstore
- Installing some packages directly from github(optional)
$go mod init go-bookstore
- Open the VS Code and make all the folders

*STAGE -II*

***ROUTES.GO FILE***

I have imported some packages i.e. gorilla/mux and pkg/controllers
This helps in getting the controller file and other file from that folder
Inside this we have a function ‘register bookstore’ this have all the routes and help in getting the controller request like GET, UPDATE AND DELETE by using GET or POST method.

***CONFIG.GO FILE***

In this file i have imported packages like gorm and MySQL which will help in connecting with the database.

***UTILS.GO FILE***

In this file i have imported packages like ioutils, encoding/json, net/http.
This will help in parsing the file into json for proper connection with the database.

***BOOK.GO FILE***

In this file i have imported packages like gorm, pkg/config.
This file helps in creating database and connecting with Mysql.

***MAIN.GO FILE***

In this file i have imported packages like log, net/http, gorilla/mux, gorm/dialects/mysql, pkg routes.
This file helps in connecting with routers.

