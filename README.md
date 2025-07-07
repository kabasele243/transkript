This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Release Process

This project uses semantic versioning and automated releases.

### Creating a Release

1. **Patch Release** (bug fixes):
   ```bash
   npm run release
   ```

2. **Minor Release** (new features):
   ```bash
   npm run release:minor
   ```

3. **Major Release** (breaking changes):
   ```bash
   npm run release:major
   ```

These commands will:
- Run tests and linting
- Build the project
- Bump the version number
- Create a git tag
- Push changes and tags to remote
- Trigger automated release workflow

### Manual Release Steps

If you need to create a release manually:

1. Ensure all changes are committed
2. Run tests: `npm run lint && npm run build`
3. Update version: `npm version [patch|minor|major]`
4. Push with tags: `git push --follow-tags`

### Automated Releases

The project includes GitHub Actions workflows:
- **CI**: Runs on every push/PR to main
- **Release**: Triggers on every push to main branch - automatically bumps version and creates GitHub releases

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
