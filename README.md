# Next.js Commerce Bagisto

A Next.js 14 and App Router-ready ecommerce template featuring:

- Next.js App Router
- Optimized for SEO using Next.js's Metadata
- React Server Components (RSCs) and Suspense
- Server Actions for mutations
- Edge Runtime
- New fetching and caching paradigms
- Dynamic OG images
- Styling with Tailwind CSS
- Checkout and payments with Bagisto
- Automatic light/dark mode based on system settings

Demo live at: [Bagisto NextJs Commerce](https://v2-bagisto-demo.vercel.app)

## Configuration

### Setup Bagisto Store

- For `BAGISTO_PROTOCOL`, `BAGISTO_STOREFRONT_ACCESS_TOKEN`, `BAGISTO_REVALIDATION_SECRET` and `BAGISTO_STORE_DOMAIN`, you need to install the [Bagisto](https://github.com/bagisto/bagisto).
- Then, you need to install the [Bagisto Headless Extension](https://github.com/bagisto/headless-ecommerce) in the Bagisto.
- Now you need to host the full application so that you have store endpoint and if you are in development mode then you can use Ngrok also.
- After that you can proceed with setting up Next.js commerce.

## Running locally

You will need to use the environment variables [defined in `.env.example`](.env.example) to run Next.js Commerce. It's recommended you use [Vercel Environment Variables](https://vercel.com/docs/concepts/projects/environment-variables) for this, but a `.env` file is all that is necessary.

> Note: You should not commit your `.env` file or it will expose secrets that will allow others to control your Bagisto store.

1. Install Vercel CLI: `npm i -g vercel`
2. Link local instance with Vercel and GitHub accounts (creates `.vercel` directory): `vercel link`
3. Download your environment variables: `vercel env pull`

```bash
pnpm install
pnpm dev
```

Your app should now be running on [localhost:3000](http://localhost:3000/).
