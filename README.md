# Nextjs App

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

## Tech

### Authentication

- Auth.js (aka NextAuth)

### Fonts and Themes

- Using Local fonts
- Check out [tailwind.config.ts](tailwind.config.ts) to see the changed themes

### Forms

- Next.js 15 new forms [docs](https://nextjs.org/docs/app/api-reference/components/form)
- allows for server side forms
- utilizes nextjs search params

### Sanity

- using markdown pluging, then add to plugins in `sanity.config.ts`
- GROQ query language
- Extract schema types with sanity's new feature
- ```ts
  npx sanity@latest schema extract --path=./sanity/extract.json
  ```
  - create new file in root `sanity-typegen.json`, and update it
  - ```bash
    npx sanity@latest typegen generate
    ```
- Sanity's live content API
- add `<SanityLive />` to `page.tsx` to render live data

### Dynamic Routes

- use square brackets in directory name ex: [id]
- destructure params to get id

### Markdown it

- used to convert markdown into a string
- [link](https://www.npmjs.com/package/markdown-it)
