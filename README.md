# Monikers

---
![Monikers](https://media.giphy.com/media/uVDhBr6CeBbQWKDesU/giphy.gif)

## Live site
[Monikers PWA](https://monikers.herokuapp.com/)

The app is best viewed on mobile. Vist the link and add the PWA to your homescreen. Android users will be given a prompt and iOS users click the share icon (box with the arrow pointing up) then scroll and click the add to homescreen button.

## Synopsis

The electronic version of your favorite party game, Monikers!

## To Setup

Window #1 - Backend

    > git clone https://github.com/daughedm/monikers.git
    > cd monikers
    > npm install

Window #2 - Frontend

    > cd monikers/client
    > npm install

Window #3 - Database

    > cd monikers
    > mkdir -p postgres/data
    > docker run --name postgres -p 5432:5432 -v $PWD/postgres/data:/var/lib/postgresql/data -e POSTGRES_PASSWORD=postgres -it postgres
    > psql -h localhost  -U postgres -W -c 'create database monikers'
    > This will prompt you for the password:  postgres
    > npm install knex -g
    > knex migrate:latest
    > knex seed:run

## To Run

Window #1 - Frontend

    > npm start

Window #2 - Backend

    > npm start
    > visit http://localhost:3000/

---

# Endpoints

## GET

### List all the cards

- GET /api/v1/cards

---

## Technologies

- Docker
- React
- Redux
- Node
- Express
- Postgres
- Knex
- Mocha
- Chai
- React-Router
- Progressive Web Application

---

### Design

---

## Contributors

[David Daugherty](https://github.com/daughedm) -
[Krista Handel](https://github.com/meloncatty) -
[Chase Richard](https://github.com/hmmChase)
