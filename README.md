[![Netlify Status](https://api.netlify.com/api/v1/badges/fba96b94-aef5-439b-a80c-773a91ef944d/deploy-status)](https://app.netlify.com/sites/hackmcgill/deploys)

![McHacks logo](https://raw.githubusercontent.com/hackmcgill/mchacks6/master/src/static/mchacks-30x48.jpg?s=200)

This is the repository for the static landing page for [HackMcGill](https://hackmcgill.com). Code based upon [boilerplate here](https://github.com/erickzhao/static-html-webpack-boilerplate).

## Setup

1.  Make sure you have [node](https://nodejs.org/en/) and [yarn](https://yarnpkg.com/lang/en/) installed.
2.  Run `yarn`.

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

- `yarn build`: Builds `/src` into `/dist`. Minifies, transpiles, etc.
- `yarn start`: Runs a build, then starts the production server from the `/dist` folder on `localhost:8080`.
- `yarn start:dev`: Starts the development server (with auto-refresh).
- `yarn deploy`: Runs a build, commits it, then deploys the `/dist` folder to the `gh-pages` branch.
- `yarn lint`: Lint scripts.
- `yarn lint:styles`: Lint stylesheets.

## Deployment

We are using Netlify to compile and host our code automatically. When a PR is created, Netlify will generate preview builds of the site to confirm that everything is working as expected. Once code is merged to `master`, Netlify will promote that code to production at `hackmcgill.com`. Netlify also handles the SSL certificate for this site. @krubenok is currently the admin on the Netlify plan. 

### Domains

The primary domain for this site (`hackmcgill.com`) is registered and has DNS with Cloudflare. It has  CNAME records pointing to `mchacks6.netlify.com` from `www.hackmcgill.com` and `hackmcgill.com `

We also have a secondary domains, `hackmcgill.ca` and `www.hackmcgill.ca` pointing to `mchacks6.netlify.com` via CNAME as above. `hackmcgill.ca` is registered with Namecheap and the DNS with Cloudflare.
