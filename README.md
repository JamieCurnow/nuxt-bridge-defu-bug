# defu-bug

This repo reproduces a bug where nuxt bridge and vite cannot find named export 'defu' in the browser in dev mode.

## Reproduction:

Clone this repo then

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev
```

Open the browser and go to http://localhost:3000 . Open the console in the browser and see the error:

```
Uncaught SyntaxError: The requested module '/_nuxt/node_modules/@nuxt/bridge/node_modules/defu/dist/defu.cjs?import' does not provide an export named 'defu' (at composables.mjs:3:10)
```
