# Movies-App

Movies-App is a web application for browsing, reviewing, and watching trailers of movies. It consists of a frontend built with React and a backend built with Spring Boot. MongoDB is used as the database.

## Features

- Browse through a list of movies
- Watch trailers of each movie
- Write and read reviews for each movie

## Project Structure

The project is divided into two main folders:

- `frontend`: Contains the React-based frontend code
- `backend`: Contains the Spring Boot-based backend code

## Prerequisites

- Node.js and npm for the frontend
- Java JDK 8 or above for the backend
- Maven or Gradle for the backend
- A modern web browser

## Getting Started

### Setting up the Database

1. Install MongoDB on your local machine. Follow the instructions [here](https://docs.mongodb.com/manual/installation/).

2. Run MongoDB:
   ```bash
   mongod
3. Seed the MongoDB database with the initial data. Navigate to the root directory where movies.json is located and run:
    ```bash
    mongoimport --db your_database_name --collection your_collection_name --file movies.json
    ```
    Replace your_database_name and your_collection_name with the appropriate values
4. If you are using a remote MongoDB instance, update the application.properties or .env file with the correct MongoDB URI.

### Setting Up the Backend

1. Navigate to the `backend` folder
    ```bash
    cd movies-app/backend
2. Build the Spring Boot project
    ```bash
    mvn clean install
3. Run the application
    ```bash
    mvn spring-boot:run
    ```
### Setting Up the Frontend

1. Navigate to the `frontend` folder
    ```bash
    cd movies-app/frontend
2. Install the necessary npm packages
    ```bash
    npm install
3. Start the React app
    ```bash
    npm start
    ```
    
## Usage

1. Open your web browser and navigate to `http://localhost:3000`
2. Browse through the available movies, watch trailers, and read or write reviews as you like.