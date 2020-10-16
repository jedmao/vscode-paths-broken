# vscode-paths-broken

Example of vscode paths broken.

See [issue #108801](https://github.com/microsoft/vscode/issues/108801).

## Instructions

Open `packages/b/src/index.ts` in vscode and "Go to Definition" on the `foo` function.

### Expected

Based on the `tsconfig.json` at root, vscode should navigate to the `foo` function within `packages/a/src/index.ts`.

### Actual

~vscode navigates to `packages/a/lib/index.js`~

Unable to reproduce.
