# OnAVote

OnAVote is a full-stack polling application for creating questions with multiple options and collecting votes.

The project uses an older but fully typed Next.js/tRPC/Prisma stack and includes separate frontend, backend, database, shared, and utility areas under `src/`.

## Implemented functionality

- authenticated poll/question creation;
- multiple options per question;
- voting;
- tRPC-based client/server communication;
- tRPC SSR support;
- Prisma-backed persistence;
- form validation and typed inputs;
- Tailwind/daisyUI interface.

The main known unfinished area in the repository is richer poll-ending behaviour such as scheduled or manual closure.

## Tech stack

- Next.js 12
- React 18
- TypeScript 4.6
- tRPC 9
- Prisma 3
- React Query
- React Hook Form + Zod
- Tailwind CSS 3 + daisyUI

## Repository structure

```text
src/
  pages/          Next.js pages/routes
  components/     UI components
  backend/        server/tRPC logic
  db/             database access
  shared/         shared contracts/utilities
  utils/          helper code
prisma/           Prisma schema/migrations
```

## Getting started

```bash
npm install
npm run dev
```

Prisma client generation runs automatically after install.

Build for production with:

```bash
npm run build
npm start
```

Configure the database and authentication environment expected by the application before exercising persisted/authenticated flows.

## Project status

OnAVote is an older proof-of-concept/full-stack project that demonstrates poll creation, voting, typed API communication, and persistence. It is intentionally documented as the implementation that exists rather than as a current-generation Next.js starter.
