# nuxt-static-deploy-appengine

Repository used for this article: https://dev.to/jlandure/3-minutes-to-deploy-your-static-nuxt-js-app-on-appengine-2a2n
See https://nuxt-static-deploy.appspot.com/

> Hello Nuxt on AppEngine 🎉

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

## Deploy setup

Don't forget to copy the file in our dist folder using this command

```
cp .appengine/app.yaml dist/.
```

Then, deploy with `gcloud`

```
gcloud app deploy --project nuxt-static-deploy dist
```
