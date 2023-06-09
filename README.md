# Introduction

Movies REST API

## The task

- Build a REST API to show movie directors

## Solutions

Here's the [Postman Collection](https://restless-meadow-827052.postman.co/workspace/My-Workspace~53eaee61-d6f5-464c-8eea-14c5e3f75563/collection/9378808-dcec59e5-1a62-4161-a54f-c1f835c7c7e3?action=share&creator=9378808)

## Tools used

- Typescript
- Node.js (Express)
- MongoDB
- Docker
- NPM

### Set up instructions

1. Clone the repository

```sh
$ git clone https://github.com/morelmiles/backend-task
```

2. Install the dependencies

```sh
$ npm install
```

3. Create a database (I use Docker on local machine)

```sh
$ docker pull mongo # Pull the mongo image from Docker Hub
$ docker run --name some-name -d mongo:tag  # Create a container
$ docker exec -it some-name sh # Terminal for the mongo container
$ root@3fdfdadd6690:/# mongosh # Launch mongo's shell
$ test> use boilerplate # Create a database named boilerplate
$ boilerplate # Database created succesfully
```

4. Copy the `env` variables and fill in the details

```sh
$ cp .env.example .env
```

5. Start the `dev` server

```sh
$ npm run dev
```

## Improvements

- Use a separate database for running tests
- Mock the database connection using `mongodb-memory-server`
- Add deployment scripts using Docker and docker-compose
