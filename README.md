# Structure

The monorepo contains two packages:

- `src`
- `example`

The `src` is a package using `ramda` and exports a simple function.
The `example` is a package that utilizes the function provided by `src`.

# Demo

Run the following command to demonstrate the issue:

```
pnpm build
```

It will build the `src` package and execute `unrun` on the `example` that will fail to import `ramda`:

> `Error [ERR_MODULE_NOT_FOUND]: Cannot find package 'ramda' imported from ...`
