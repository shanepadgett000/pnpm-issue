# Demonstrate the error with frozen-shrinkwrap and shamefully-flatten.

Both projects have a `.npmrc` file with the settings that show the problem. In both projects simply run:

```bash
pnpm i
```

## Results

The worming directory will fail because the dependency has been updated in the package.json. The flat-node-modules directory will not fail to install, and will update the package.json.