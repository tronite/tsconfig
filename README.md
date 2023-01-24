# @tarrasque/tsconfig

This package provides [TypeScript](https://www.typescriptlang.org/) configuration for [Tarrasque App](https://tarrasque.app) projects.

## Installation

```sh
yarn add --dev @tarrasque/tsconfig
```

## Usage

Add the following to your `tsconfig.json` file, depending on your project type:

### Next.js

```json
{
  "extends": "@tarrasque/tsconfig/nextjs.json"
}
```

### NestJS

```json
{
  "extends": "@tarrasque/tsconfig/nestjs.json"
}
```

### React

```json
{
  "extends": "@tarrasque/tsconfig/react.json"
}
```

### ESM

```json
{
  "extends": "@tarrasque/tsconfig/esm.json"
}
```
