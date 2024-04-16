# PNPM bug report

To trigger the bug:

```bash
pnpm --version # should be 9.0.0
pnpm -C app1 install --frozen-lockfile # observe that it doesn't respect the packageManager attribute in the package.json
cd app1 && pnpm install --frozen-lockfile # works
```
