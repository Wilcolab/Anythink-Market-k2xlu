# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

### Prerrequisites

- Install docker [Docker](https://www.docker.com/)

### Run the app

- `docker compose build`
- `docker compose up`

Once the app is running, use the following command to setup the database:

- `docker compose exec -w /usr/src/backend anythink-backend bin/rails db:migrate`
- `docker compose exec -w /usr/src/backend anythink-backend bin/rails db:seed`

Then use the following url to access the app:

[http://localhost:3001](http://localhost:3001)
