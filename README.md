# Campus Events

A learning project for building a Campus Events application with Angular and an Express API.

## Project status

- The Express API manages campus events in memory.
- Events can be listed, searched by title, filtered by start date, sorted by date or title, created, updated, and deleted.
- `GET /api/stats` reports the event count, total capacity, and earliest future event.
- Event input is validated on the server. Requests are logged after their responses finish.
- The Angular client is currently a starter interface with the Lab 01 counter; it is not yet connected to the events API.

## Run the API

From a terminal:

```sh
cd server
npm install
npm run dev
```

The API listens at `http://localhost:3000`. The development command restarts the server when source files change. Events are stored only in memory, so restarting resets them to the initial sample events.

## Try the requests

Open `server/requests.http` in Visual Studio Code with a REST client extension and send the requests individually. Some requests depend on earlier ones. Follow the comments in the file, including the point where the server must be restarted.

## Run the Angular starter client

In a second terminal:

```sh
cd client
npm install
npm start
```

The client is served at `http://localhost:4200`.
