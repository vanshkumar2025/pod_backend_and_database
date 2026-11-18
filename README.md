# CollabSpace backend and database

PostgreSQL is required. Prisma migrations create the relational schema.

## Local setup

```bash
cp .env.example .env
npm install
npm run db:up
npm run db:migrate
npm run dev
```

Then run the API with `npm start` (serves the built frontend) or keep Vite on `npm run dev` and point the app at the Node server.

`DATABASE_URL` must be a PostgreSQL connection string, for example:

`postgresql://collabspace:collabspace@localhost:5432/collabspace?schema=public`
