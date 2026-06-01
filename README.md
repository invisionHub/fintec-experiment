# Fintech Nest API

A NestJS-based fintech API for managing user accounts, wallets, transactions, and admin reporting.

## Features

- User registration and authentication
- Wallet creation and management
- Deposit funds, transfer funds, withdraw funds
- Transaction history and audit trails
- Portfolio analytics and balance summaries
- Notifications and failed notification retry handling
- Admin features: view transactions, reconciliation reports, system health monitoring, audit logs

## Tech stack

- Node.js
- TypeScript
- NestJS
- Jest for tests
- ESLint + Prettier for linting and formatting

## Getting started

### Prerequisites

- Node.js 20+ (or compatible version)
- npm 10+ (or yarn)
- PostgreSQL / MySQL / preferred database configured for the API

### Install dependencies

```bash
npm install
```

### Configure environment

Create a local `.env` based on the example file:

```bash
cp .env.example .env
```

For environment-specific examples, see:

- `config/.env.dev.example`
- `config/.env.staging.example`
- `config/.env.prod.example`

### Run in development

```bash
npm run start:dev
```

### Build for production

```bash
npm run build
npm run start:prod
```

## Environment variables

This repository uses environment variables for configuration. Copy `.env.example` to `.env` and update values for your environment.

Example variables:

```env
APP_PORT=3000
NODE_ENV=development
DATABASE_URL=postgresql://user:password@localhost:5432/fintech_db
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=3600s
SMTP_HOST=smtp.example.com
SMTP_PORT=587
SMTP_USER=example-user
SMTP_PASS=example-pass
NOTIFICATION_PROVIDER_API_KEY=your_api_key
ENABLE_AUDIT_LOGS=true
CORS_ORIGINS=http://localhost:3000
```

## Scripts

```bash
npm run start           # run production server via Nest
npm run start:dev       # run server in watch mode
npm run start:prod      # run compiled production server
npm run build           # compile TypeScript
npm run lint            # lint and autofix
npm run format          # format source files
npm run test            # run unit tests
npm run test:e2e        # run end-to-end tests
npm run test:cov        # coverage report
```

## Project structure

- `src/` — application source code
- `test/` — end-to-end tests
- `tsconfig.json` / `tsconfig.build.json` — TypeScript configuration
- `eslint.config.mjs` — linting rules

## Contributing

Please read [`CONTRIBUTING.md`](CONTRIBUTING.md) before opening issues or pull requests.

## Reporting issues

Use the issue templates in `.github/ISSUE_TEMPLATE/` for bug reports and feature requests.

## Notes

- Keep secrets out of Git.
- Use the environment-specific example files for staging and production.
- Ensure all new endpoints are covered by tests before merging.
