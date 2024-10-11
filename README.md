# Sniplee Config

Sniplee Config provides standardized configuration packages for TypeScript, Biome, and more. 

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Available Configurations](#available-configurations)
- [Example](#example)

## Installation

Install `sniplee-config` using your preferred package manager. This package includes configurations for a variety of tools commonly used in our open-source projects.

```bash
npm install sniplee-config
pnpm add sniplee-config
yarn add sniplee-config
```

# Usage

After installing sniplee-config, extend your project’s configuration files by referencing the desired presets. Use the following convention to extend configurations:

```
sniplee-config/<config-name>
```
Checkout [Available Configurations](#available-configurations) for `config-name`.

# Available Configurations
This package includes the following configurations:

- [`sniplee-config/typescript`](./src/tsconfig.json)
- [`sniplee-config/biome`](./src/biome.json)

## Example
To extend the TypeScript configuration in your `tsconfig.json`
```json
{
    "extends": ["sniplee-config/typescript"],
    "compilerOptions": {
        "outDir": "dist",
        "rootDir": "src"
    }
}
```

