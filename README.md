https://user-images.githubusercontent.com/43780137/158059050-481ffa30-e415-4156-aea7-072c817f2ae2.mp4

[![Version](https://img.shields.io/static/v1?label=version&message=2.0.0&color=blue)](https://shields.io/)
[![NPM](https://img.shields.io/static/v1?label=npm&message=6.8.5&color=blue)](https://shields.io/)
[![NODE](https://img.shields.io/static/v1?label=node&message=10.12.8&color=success)](https://shields.io/)
[![MYSQL](https://img.shields.io/static/v1?label=mysql&message=8.0.10&color=blueviolet)](https://shields.io/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://shields.io/)



## My Tech Stack (MERN)

#### Front-end

- Front-end Framework: `React.js (with Redux)`
- Styling: `SASS` and `BOOTSTRAP`

#### Back-end

- For handling index requests: `Node.js with Express.js Framework`
- As Database: `MySQL with Sequelize`
- API tested using: `POSTMAN`

## Guidelines to setup

There are two ways to setup the project: manually or using the Dockerfile. Read below for more details:

### Manual Setup

1. Open your local CLI -

   ```
   mkdir Stackoverflow-Clone
   cd Stackoverflow-Clone
   ```

2. Setup the backend code -
   
   __NOTE:__ For Frontend Developers, if they dont want to setup the Backend Code, they can skip the Step 2, and make sure they follow the optional step mentioned in Step 4

   - Create a `.env` file and the format should be as given in `.env.example`.
   - Clone the code & install the modules-

     ```
     git clone https://github.com/Mayank0255/Stackoverflow-Clone-Backend.git
     cd Stackoverflow-Clone-Backend

     npm install
     ```

   - Open your MySQL Client -

     ```
     CREATE DATABASE stack_overflow;
     ```
     NOTE: Don't forget to keep the database name same in the `.env` and here.

   - Run the index `npm start`.

3. Open a new CLI terminal and goto the root `Stackoverflow-Clone` folder you created in the first step.
4. Setup the Frontend code -

   - Clone the code & install the modules-

     ```
     git clone https://github.com/Mayank0255/Stackoverflow-Clone-Frontend.git
     cd Stackoverflow-Clone-Frontend

     npm install
     ```

   - Run the client index `npm start`.
Let me know if you are interested and would want me to assign it to you

### Docker Setup

The back-end has support for Docker. So if you want to run the back-end in a container, you need do:

- Setup environment variables in `.env` file. Note when you use Docker setup and run the database in localhost (host machine), you need to setup the environment variables for use correct IP of MySQL Database. 
- Build the Docker image:
  ```
  docker build -t stackoverflowclone .
  ```
- Run the container. For example, if you want to run the container in a new terminal, you can do:
  ```
  docker run -d -p 5000:5000 stackoverflowclone
  ```

The default port of api is 5000. After running the container, you can access the api by typing:

    http://localhost:5000/api/<endpoint that you request - see next section>

_Follow the steps properly (manual or Docker) and you are good to go._

