# Next.JS `index` page issue

This code was generated using:
```
yarn create next-app --typescript
```
and the experimental `app` feature enabled.

Then the `<root>/src/app/index/page.tsx` and `<root>/src/app/notindex/page.tsx` were added with simple content:
```
export default function NotIndex() {
  return (
    <div>You can see me!</div>
  )
}
```

Finally run `yarn dev` and navigate to:
- http://localhost:3000 --> No problem
- http://localhost:3000/notindex --> No problem
- http://localhost:3000/index --> Problem: seems to load for ever and browser gives up with "Connection refused." error
