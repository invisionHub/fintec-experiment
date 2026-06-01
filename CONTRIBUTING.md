# Contributing to Fintech Nest API

Thank you for contributing to this fintech API project. Your feedback, bug reports, and code contributions help make this application more reliable and maintainable.

## How to contribute

1. Fork the repository and create a branch named for your work:
   - `feature/<short-description>`
   - `bugfix/<short-description>`

2. Install dependencies:

```bash
npm install
```

3. Create or update environment files from examples:

```bash
cp .env.example .env
```

4. Run tests locally before submitting changes:

```bash
npm run test
npm run test:e2e
```

5. Keep your changelist focused and add tests for new behavior.

## Code style

- Use TypeScript and follow existing NestJS patterns.
- Run lint and formatter before committing:

```bash
npm run lint
npm run format
```

- Write clean, self-documenting code.
- Keep functions and files small and focused.
- Add or update tests for bug fixes and features.

## Branching and pull requests

- Base your branch on `main`.
- Open a pull request with a clear title and summary.
- Reference related issue numbers when relevant.
- Include tests and explain how to verify the change.

## Issues

Use the issue templates in `.github/ISSUE_TEMPLATE/` when reporting bugs or requesting features.

### Bug reports

Include:

- steps to reproduce
- actual vs expected behavior
- environment details
- logs or error messages

### Feature requests

Describe:

- the problem you want solved
- the desired behavior
- acceptance criteria

## Security

If you find a security issue, do not open a public issue. Contact the repo maintainers directly or use a private channel.

## Thank you

Thanks for improving the Fintech Nest API. Every contribution makes the application stronger.
