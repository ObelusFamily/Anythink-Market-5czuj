# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

- [Install Docker](https://docs.docker.com/get-docker/)
- Verify Docker is working with `docker -v` and `docker-compose -v`. Both are required to proceed.
- From the project root run `docker-compose up`. This will start run the application with 3 containers - backend, frontend, and mongo database
- To confirm the backend is running, go to http://localhost:3000/api/ping. You should get a 200 response a message that everything is working.
- To confirm teh backend can talk to the frontend and database, go to http://localhost:3001/register and register yourself as a new user.
