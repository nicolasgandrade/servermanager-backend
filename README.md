# Server Manager - Backend
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)

<p id="objective"> A backend API to manage servers: add servers, delete and ping them.  
This API is a part of a Fullstack application, so it is being consumed by the frontend app. You can find the frontend repository here: https://github.com/nicolasgandrade/servermanager-frontend </p>

<h4 align="center"> 
	🚧  Server Manager 🚀 In the last adjustments to be deployed...  🚧
</h4>

<p align="center">
 <a href="#objective">Objective</a> •
 <a href="#features">Features</a> •
 <a href="#start">Getting started</a> • 
 <a href="#endpoints">Endpoints</a> •  
 <a href="#author">Author</a>
</p>

<h2 id="features">Features</h2>

- [x] Save new server
- [x] Delete server
- [x] Ping server

  
<h2 id="start">Getting started</h2>
1. Clone the application to your local machine, and open the project in your favorite IDE (must be compatible to Spring Boot).  <br>
2. In the last lines of ServerResource.java change the return statement to the path you have downloaded the images you're gonna use to the UI. <br>
3. Create a database on PostgreSQL called "servermanager", or change the configs at application.properties.  <br>
4. Now you can run and access in your default Spring Boot port.  <br>
<br>
To test the API manually, you can use Postman, Insomnia or similar and try the endpoints.

<h2 id="endpoints">Endpoints</h2>

1. Return a list of all the servers (GET)
```
/servers/list
```
<br>

2. Return a server by id (GET)
```
/servers/get/{id}
```
<br>


3. Save a new server (POST)
```
/servers/save
```
JSON example:
```
{
  "ipAddress": "string",
  "name": "string",
  "memory": "string",
  "type": "string",
  "imgUrl": "string",
  "status": SERVER_DOWN
}
```
<br>

4. Ping a server (GET)
```
/servers/ping/{ipAddress}
```
<br>

5. Delete a server by id (POST)
```
/servers/delete/{id}
```
<br>

<h3 id="author">Author</h3>
<hr>

<img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/82426254?s=120&v=4" width="100px;" alt=""/>
Made with ❤️ by Nicolas Guerrero 👋