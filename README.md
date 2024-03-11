# Fullstack Notes App

Full stack notes app: where you add, delete and update notes.
The notes are persistant between refreshes because of the database integration.

## Technologies Used

Frontend: React + CSS
Backend: Node.js
Language: Typescript
Database: PostgreSQL

### Endpoints

- `GET /api/notes`: Retrieve all notes.
- `POST /api/notes`: Add a new note.
- `DELETE /api/notes/:id`: Delete a note by ID.
- `PUT /api/notes/:id`: Update a note by ID.

## Database Schema

The following Prisma schema represents the database model used to store notes:

```prisma
model Note {
  id      Int     @id @default(autoincrement())
  title   String
  content String
}
```

## Additional Infomration

Storing notes to Postgres Database
[text](https://www.elephantsql.com/)

Used Prisma to talk to the database without needing to write SQL commands.
[text](https://www.prisma.io/docs/orm/prisma-client)

Used CORs for bypassing cors issues while developing locally.

Express framwork used to create the API endpoints and handles the requests.
[text](https://expressjs.com/)