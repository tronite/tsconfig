<div align="center">
  <a href="https://tronite.com.app" target="_blank"><img src="https://tronite.com/images/logo.png" width="150" /></a>
  <h1>@tronite/tsconfig</h1>
</div>

This package provides [TypeScript](https://www.typescriptlang.org/) configuration for [Tronite](https://tronite.com) projects. It is intended to be used with [@tronite/eslint-config](https://github.com/tronite/eslint-config) and [@tronite/prettier-config](https://github.com/tronite/prettier-config).

## Installation

To install this package, run the following command:

```sh
yarn add --dev @tronite/tsconfig
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
  "extends": "@tronite/tsconfig/nextjs",
  "include": ["**/*.ts", "**/*.tsx"],
  "exclude": ["node_modules", ".next"]
}
```

### NestJS

```json
{
  "extends": "@tronite/tsconfig/nestjs",
  "include": ["**/*.ts"],
  "exclude": ["node_modules", "dist"]
}
```

### React

```json
{
  "extends": "@tronite/tsconfig/react",
  "include": ["**/*.ts", "**/*.tsx"],
  "exclude": ["node_modules", "dist"]
}
```

### ESM

```json
{
  "extends": "@tronite/tsconfig/esm",
  "include": ["**/*.ts", "**/*.mts"],
  "exclude": ["node_modules", "dist"]
}
```
