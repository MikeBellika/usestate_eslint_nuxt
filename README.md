# ESLint useState reproduction

This repo shows that `vue/no-ref-as-operand` doesn't pick up on `useState` being used without `.value`.

To reproduce run:

```bash
pnpm install && pnpm lint
```

You should see that line 9 gives an error with the `ref`, but line 4 doesn't
