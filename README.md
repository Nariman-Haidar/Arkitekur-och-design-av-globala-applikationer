# Arkitekur-och-design-av-globala-applikationer
# IV1201 Backend

Backend server deployed on heroku. This project is the backend component of a recruitment application, developed using JAVA. For developing and testing you also need to have a database running locally.

## How to run the app in localhost 

### Git clone
```
$ git clone  
$ cd IV1201
$ npm install
```
###  Database Setup
Create a local database using PostgreSQL: run the script found in the root folder to create the database with the specified tables.

### Configuration
Update the application.properties file located in the resource folder:
```
$ spring.datasource.url=jdbc:postgresql://localhost:YOUR_DB_PORT/YOUR_DB_NAME
$ spring.datasource.username=YOUR_USERNAME
$ spring.datasource.password=YOUR_PASSWORD
```
### Change JwtUtil.java file located in the security folder:
```
$ @Value("${JWT_SECRET_KEY}") comment out this line
private String secretKey = "SET YOUR TESTING SECRET";

$ @Value("${JWT_EXPIRATION}") comment out this line
private long expiration = SET A LENGTH;
```

### Usage
Before starting the backend server, ensure that the database are running.

# IV1201_frontend
React app frontend deployed on heroku. This project is the frontend component of a recruitment application, developed using React. It encompasses essential dependencies for both testing and development purposes.

## Installation
### Clone the repository:
```
$ git clone 
$ cd frontend
$ npm install
```
### Navigate into the project directory:
```
$ cd frontend
```
### Create a .env file: 
In the root directory of the frontend, create a .env file and add the following environment variable, replacing YOUR_BACKEND_URL with the URL of your backend:
```
$ REACT_APP_BACKEND_URL=YOUR_BACKEND_URL
```
### Install dependencies:
```
$ npm install
```
## Usage
Before starting the frontend server, ensure that the backend and database are running.

To start the development server, run:
```
$ npm start
```

