# bobOS

An AI chat application built around the bobo character and community, combining a custom web interface with an Express agent service.

## Highlights

- Next.js and React interface with Solana wallet integration.
- Server-side wallet signature verification.
- Gemini model routing with fallback handling and request timeouts.
- Token-gated chat experiences and character context.
- Shared PostgreSQL data layer using Drizzle ORM.

## Repository map

| Path | Purpose |
| --- | --- |
| [apps/web](apps/web) | Next.js interface and server actions |
| [apps/agent](apps/agent) | Express agent, model integration, and chat workflows |
| [packages/database](packages/database) | Shared database package |

## Development

The workspace uses **pnpm 9.15.4**. Install dependencies, configure PostgreSQL and the provider environment variables, then start the workspace:

```bash
pnpm install
pnpm dev
```

Use [the agent environment example](apps/agent/.env.example) as a configuration reference. Supply real credentials through your local environment or deployment provider.

Other workspace commands:

```bash
pnpm build
pnpm typecheck
```

## Project focus

This repository demonstrates interface development, LLM integration, wallet authentication, and a shared application data layer.

Built by [Alejandro Mendoza / bobo labs](https://github.com/bobo-labs).
