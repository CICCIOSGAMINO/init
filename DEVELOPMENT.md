# Development

Getting the code
================



1.  Fork the repo.
2.  Clone your fork.
3.  Install [Node](https://nodejs.org/en/download/). It comes bundled with [yarn](https://yarnpkg.com/).
4.  Install the [dependencies](#dependencies)

## Dependencies

Project dependencies are managed through [Yarn](https://yarnpkg.com/lang/en/docs/install).

Install dependencies with:

```sh
yarn
```

## Serve
We use [ed dev server](https://github.com/open-wc/open-wc/tree/master/packages/es-dev-server) a web server for development without bundling. 

```bash
# use the server without install it 
npx es-dev-server --node-resolve --watch

# install 
npm i --save-dev es-dev-server
```

Add scripts to your package.json, modify the flags as needed:

```json
{
  "scripts": {
    "start": "es-dev-server --app-index index.html --node-resolve --watch --open"
  }
}
```

And run the server: 

```bash
npm run start
```

## Viewing the element

First analyze the projcet then start up the included local webserver:

```sh
yarn run analyze
yarn run serve
```

Then visit http://127.0.0.1:8000

Please note that as this is an unbuild version of the docs, not all browser will be able to view the page. To view the built version of the docs see [Docs](#docs)

## Building

Build with:

```sh
yarn run build
```

## Coding Style

```sh
yarn run lint
```

## Docs


## Testing
