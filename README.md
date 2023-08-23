# `next@12` with `@auth0/nextjs-auth0@3`

**This repo is to demonstrate that `@auth0/nextjs-auth0@3` is expecting `next@13`. See https://github.com/auth0/nextjs-auth0/issues/1393.**

It has `next@12` and `@auth0/nextjs-auth0@3` installed. It includes a `/pages/middleware.js` to require authentication on all pages. If you install the dependencies, run the dev server, and load a page, you will see the following:

```
Module not found: Can't resolve 'next/navigation'

Import trace for requested module:
./node_modules/@auth0/nextjs-auth0/dist/helpers/index.js
./node_modules/@auth0/nextjs-auth0/dist/edge.js
./middleware.js

https://nextjs.org/docs/messages/module-not-found
```

`@auth0/nextjs-auth0@3` is using `next@13` features but currently lists `next@>=10` as a peer dependency.

<hr />

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
