![McHacks logo](https://raw.githubusercontent.com/hackmcgill/mchacks6/master/src/static/mchacks-30x48.jpg?s=200)

This is the repository for the static landing page for [HackMcGill](https://hackmcgill.com). Code based upon [boilerplate here](https://github.com/erickzhao/static-html-webpack-boilerplate).

## Setup
1. Make sure you have [node](https://nodejs.org/en/) and [yarn](https://yarnpkg.com/lang/en/) installed.
2. Run `yarn`.

## Folder structure
```
📁dist        -- contains production-ready code
📁src         -- source code folder
|--📁js       -- script files
|--📁static   -- static assets (images, fonts, etc.)
|--📁style    -- SCSS style sheets
...
```
## Available scripts
* `yarn build`: Builds `/src` into `/dist`. Minifies, transpiles, etc.
* `yarn start`: Runs a build, then starts the production server from the `/dist` folder on `localhost:8080`.
* `yarn start:dev`: Starts the development server (with auto-refresh).
* `yarn deploy`: Runs a build, commits it, then deploys the `/dist` folder to the `gh-pages` branch.
* `yarn lint`: Lint scripts.
* `yarn lint:styles`: Lint stylesheets.
