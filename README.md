# WORKING example of a monorepo with prisma - deployed to vercel

Link to full Prisma monorepo docs

https://www.prisma.io/docs/guides/turborepo


## Dev mode
Start postgres database (via Docker)

`pnpm run db:up`

Migrate database

`pnpm run db:migrate`


Run web apps

`pnpm run dev`

## Prod mode
Run the custom build command to deploy the database and generate prisma client before building

`pnpm run vercel-build`

(If using vercel, override the vercel project's default command with this one.)
