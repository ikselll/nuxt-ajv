# nuxt-ajv

## Reproduction steps

```bash
# install dependencies
$ npm install

# run check-peer-dependencies
$ npm run show-issue
```

## Error

```bash
nuxt-ajv git:(master) ✗ npm run show-issue

> nuxt-ajv@1.0.0 show-issue
> npx check-peer-dependencies

  ✅  ajv ^6.9.1 is required by ajv-keywords@3.5.2 (6.12.6 is installed)
  ✅  ajv >=5.0.0 is required by ajv-errors@1.0.1 (6.12.6 is installed)
  ❌  ajv ^8.8.2 is required by ajv-keywords@5.1.0) (6.12.6 is installed)

Search for solutions using this command:

npx check-peer-dependencies --findSolutions

Install peerDependencies using this command:

npx check-peer-dependencies --install

➜  nuxt-ajv git:(master) ✗ npx check-peer-dependencies --findSolutions
  ✅  ajv ^6.9.1 is required by ajv-keywords@3.5.2 (6.12.6 is installed)
  ✅  ajv >=5.0.0 is required by ajv-errors@1.0.1 (6.12.6 is installed)
  ❌  ajv ^8.8.2 is required by ajv-keywords@5.1.0) (6.12.6 is installed)

Searching for solutions for 1 missing dependencies...

  ❌  Unable to find a version of ajv that satisfies the following peerDependencies: ^6.9.1 and >=5.0.0 and ^8.0.0 and ^8.8.2
```
