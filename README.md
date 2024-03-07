# Nuxt Token Authentication

[![npm version][npm-version-src]][npm-version-href]
[![npm downloads][npm-downloads-src]][npm-downloads-href]
[![License][license-src]][license-href]
[![Nuxt][nuxt-src]][nuxt-href]

Token Authentication for Nuxt server APIs for doing amazing things.

- [✨ &nbsp;Release Notes](/CHANGELOG.md)
  <!-- - [🏀 Online playground](https://stackblitz.com/github/your-org/nuxt-token-authentication?file=playground%2Fapp.vue) -->
  <!-- - [📖 &nbsp;Documentation](https://example.com) -->

## Features

<!-- Highlight some of the features your module provide here -->

- ⛰ &nbsp;Foo
- 🚠 &nbsp;Bar
- 🌲 &nbsp;Baz

## Quick Setup

1. Add `nuxt-token-authentication` dependency to your project

```bash
# Using pnpm
pnpm add -D nuxt-token-authentication

# Using yarn
yarn add --dev nuxt-token-authentication

# Using npm
npm install --save-dev nuxt-token-authentication
```

2. Add `nuxt-token-authentication` to the `modules` section of `nuxt.config.ts`

```js
export default defineNuxtConfig({
  modules: ["nuxt-token-authentication"],
  nuxtTokenAuthentication: {
    tokenHeader: "Token",
    noAuthRoutes: ["POST:/api/auth/getToken"],
  },
});
```

3. Set Prisma schema

Set it from command line: https://www.prisma.io/docs/orm/reference/prisma-cli-reference#init

3.1. `npx prisma init` to create a new Prisma schema file or use an existing one.

3.2. In your `/.env` file, set the `DATABASE_URL` environment variable to point to your existing database. If your database has no tables yet, read [Getting Started with Prisma](https://pris.ly/d/getting-started).

```env
DATABASE_URL="postgresql://johndoe:randompassword@localhost:5432/mydb?schema=public"
```

3.3. Set the provider of the datasource block in schema.prisma to match your database: postgresql, mysql, sqlite, sqlserver, mongodb or cockroachdb.

3.4. Run `npx prisma db pull` to turn your database schema into a Prisma schema.

TODO `npx prisma db push` and seeding `npx prisma db seed`

3.5. Run `npx prisma generate` to generate the Prisma Client. You can then start querying your database.

That's it! You can now use Nuxt Token Authentication in your Nuxt app ✨

## Development

```bash
# Install dependencies
npm install

# Generate type stubs
npm run dev:prepare

# Develop with the playground
npm run dev

# Build the playground
npm run dev:build

# Run ESLint
npm run lint

# Run Vitest
npm run test
npm run test:watch

# Release new version
npm run release
```

<!-- Badges -->

[npm-version-src]: https://img.shields.io/npm/v/nuxt-token-authentication/latest.svg?style=flat&colorA=020420&colorB=00DC82
[npm-version-href]: https://npmjs.com/package/nuxt-token-authentication
[npm-downloads-src]: https://img.shields.io/npm/dm/nuxt-token-authentication.svg?style=flat&colorA=020420&colorB=00DC82
[npm-downloads-href]: https://npmjs.com/package/nuxt-token-authentication
[license-src]: https://img.shields.io/npm/l/nuxt-token-authentication.svg?style=flat&colorA=020420&colorB=00DC82
[license-href]: https://npmjs.com/package/nuxt-token-authentication
[nuxt-src]: https://img.shields.io/badge/Nuxt-020420?logo=nuxt.js
[nuxt-href]: https://nuxt.com
