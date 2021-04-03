# transpilation-free-starter-kit

This repo contains an example of how to create an application with jsx-like syntax and type checking without transpilation.

## Motivation

Let's return to the basics when we just update files and refresh the page without bundlers.

## Getting Starting

Clone the repo, install dependencies and start a static server:

```bash
git clone git@github.com:petersolopov/transpilation-free-starter-kit.git
npm install
npm run serve
```

**Important**: Open link in browsers with [`import maps` supporting](https://caniuse.com/import-maps).

## How It Works

- It uses [htm](https://github.com/developit/htm) for jsx-like syntax.
- Control javascript imports with [import-maps](https://github.com/wicg/import-maps)
- Type checking javascript files with [typescript + jsdocs](https://www.typescriptlang.org/docs/handbook/jsdoc-supported-types.html).

## Building App

You should build your app once for production:

```
npm run build
```

[93% of users](https://caniuse.com/es6-module) are now running browsers with support for ES modules. That's why it creates two versions of the app: ES6 modules for modern browsers and SystemJS modules for legacy browsers.

**Supports**: IE11 and all modern browsers.

## LICENSE

[MIT](/LICENSE)
