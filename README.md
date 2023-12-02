## TLDR
- cool setup with nextjs.
- to use redux selector and dispatch: useAppSelector and useAppDispatch
- for ui and style: tailwind lucide and shadcn

## What's this
- this quick setup for nextjs with tailwind, redux, shadcn, and lucide-react.
- from shadcn the Button and Input component are already added with the purple theme (to change the theme) just go into src/app/global.css and change the variable values inside :root
- all file regarding redux are into src/lib/redux the store is provided in a component inside this folder called ReduxStoreProvider that just provide the store and load children, this componend is rendered in src/app/layout.tsx. for the selector and dispatch there are 2 custom hooks which are called useAppSelector and useAppDispatch, they work the same as their normal counterpart but are typed.
- there is also a function in utils called cn that is used by shadcn, it's just a function that use tailwind-merge and clsx together you can also use it into component to have the className loaded better (don't move or delete this file or the function in it, you can add other function if you want but leave the cn function where it is as it is used by shadcn)


# Nextjs default readme

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

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

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
