<div align="center">
  <a href="https://tarrasque.app" target="_blank"><img src="https://tarrasque.app/images/logo.svg" width="150" /></a>
  <h1>@tarrasque/tsconfig</h1>
</div>

This package provides [TypeScript](https://www.typescriptlang.org/) configuration for [Tarrasque App](https://tarrasque.app) projects. It is intended to be used with [@tarrasque/eslint-config](https://github.com/tarrasqueapp/eslint-config) and [@tarrasque/prettier-config](https://github.com/tarrasqueapp/prettier-config).

## Installation

To install this package, run the following command:

```sh
yarn add --dev @tarrasque/tsconfig
```

You will also need to install the following peer dependencies:

```sh
yarn add --dev typescript
```

## Usage

Add the following to your `tsconfig.json` file, depending on your project type:

### Next.js

```json
{
  "extends": "@tarrasque/tsconfig/nextjs",
  "include": ["**/*.ts", "**/*.tsx"],
  "exclude": ["node_modules", ".next"]
}
```

### NestJS

```json
{
  "extends": "@tarrasque/tsconfig/nestjs",
  "include": ["**/*.ts"],
  "exclude": ["node_modules", "dist"]
}
```

### React

```json
{
  "extends": "@tarrasque/tsconfig/react",
  "include": ["**/*.ts", "**/*.tsx"],
  "exclude": ["node_modules", "dist"]
}
```

### ESM

```json
{
  "extends": "@tarrasque/tsconfig/esm",
  "include": ["**/*.ts", "**/*.mts"],
  "exclude": ["node_modules", "dist"]
}
```
