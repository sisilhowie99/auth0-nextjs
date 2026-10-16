# Auth0 Next.js

A basic Next.js app demonstrating authentication with Auth0, built by following the [Auth0 Next.js SDK](https://github.com/auth0/nextjs-auth0) documentation.

## Features

- Login/logout via Auth0
- Protected home page that redirects unauthenticated users to `/auth/login`
- Displays the logged-in user's profile

## Getting Started

### 1. Install dependencies

```bash
npm install
```

### 2. Configure environment variables

Create a `.env.local` file in the project root with your Auth0 application credentials:

```bash
AUTH0_DOMAIN=
AUTH0_CLIENT_ID=
AUTH0_CLIENT_SECRET=
AUTH0_SECRET=
APP_BASE_URL=http://localhost:3000
```

See the [Auth0 Next.js SDK docs](https://github.com/auth0/nextjs-auth0) for how to obtain these values.

### 3. Run the dev server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

- `src/app` - App Router pages and layout
- `src/components` - Login/logout buttons and profile display
- `src/lib/auth0.ts` - Auth0 client instance
- `src/proxy.ts` - Auth0 middleware for handling auth routes
