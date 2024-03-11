# Fullstack Notes App

Full stack notes app: where you can add, delete and update notes.
The notes are persistant between refreshes because of the database integration.

## Preview


## Technologies Used

- Frontend: React + CSS
- Backend: Node.js
- Language: Typescript
- Database: PostgreSQL

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

Used [Elphant SQL](https://www.elephantsql.com/) to host the Postgres SQL database.

Used [Prisma](https://www.prisma.io/docs/orm/prisma-client) to talk to the database without needing to write SQL commands.

Used [Express](https://expressjs.com/) framework used to create the API endpoints and handles the requests.