# @diegopluna/biome-config

<p>
    <img alt="npm version" src="https://img.shields.io/npm/v/%40diegopluna%2Fbiome-config?style=for-the-badge&logo=npm">
    <img alt="biome version" src="https://img.shields.io/github/package-json/dependency-version/diegopluna/biome-config/peer/%40biomejs%2Fbiome?style=for-the-badge&logo=biome">
    <img alt="downloads" src="https://img.shields.io/npm/dy/%40diegopluna%2Fbiome-config?style=for-the-badge">
</p>

## Usage

### Installation

```bash
npm install -D @diegopluna/biome-config
```

### Configuration

Add the following to your `biome.json` file:

If it's a Node.js project:

```jsonc
// <project-root>/biome.json
{
   "extends": ["@diegopluna/biome-config/node"]
}
```

If it's a React project:

```jsonc
// <project-root>/biome.json
{
   "extends": ["@diegopluna/biome-config/react"]
}
```

### Scripts

Add the following to your `package.json` file:

```json
{
  "scripts": {
    "lint": "biome lint .",
    "lint:fix": "biome lint . --apply"
  }
}
```

### VSCode Configuration

1. Install the [Biome extension](https://marketplace.visualstudio.com/items?itemName=biomejs.biome) for VSCode.
2. Create a `.vscode/settings.json` file in your project with the following content:

```json
{
  // ...
  "editor.defaultFormatter": "biomejs.biome",
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "quickfix.biome": "explicit",
    "source.organizeImportes.biome": "explicit"
  },
  // ...
}
```
