# NoteHub

NoteHub is a Next.js App Router application for creating, searching, and
managing personal notes.

## Getting started

1. Install dependencies with `npm ci`.
2. Copy `.env.example` to `.env.local`.
3. Set `NEXT_PUBLIC_NOTEHUB_TOKEN` in `.env.local` to your NoteHub API token.
4. Run `npm run dev` and open <http://localhost:3000>.

The notes list and note details are server-prefetched with TanStack Query and
hydrated for the client. Note creation, deletion, and search are handled on the
client.

## Production deployment

Deploy this project with Vercel and set `NEXT_PUBLIC_NOTEHUB_TOKEN` in the
project's Environment Variables for the Production environment before
deploying. The variable must be available at build time. After deployment,
verify the home page, notes list, note details, and create/delete flows.

## Validation

- `npm run lint`
- `npm run build`
