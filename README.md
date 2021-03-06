# deployable

Deployable helps teams deploy their projects easily. It helps you create Heroku-like application builds using [buildpacks](https://devcenter.heroku.com/articles/buildpacks) while giving you the ability to do [Deployinator](https://github.com/etsy/deployinator)-esque one-click & easy deploys.

Deployable has a couple of opinions about deploys:
* Repositories must be different staging and production environments
* Builds are done automatically from GitHub webhooks
* Staging environments _should_ be automatically deployed on successful builds
* Heroku Cedar-14 environments; your architecture should be language & application independent
* Confirmation from each author in order to deploy to production

## Setup

You'll need to create a [GitHub application key](https://github.com/settings/developers). Once you have this, you will then need to create a `.env` file on the root directory of the project.

```
URL=https://deployable.ngrok.com
GITHUB_CLIENT_KEY=
GITHUB_CLIENT_SECRET=
```

Then, make sure you have [Node.js](https://nodejs.org/en/) installed on your machine. Afterwards, you can run `npm install` which install all dependencies and build the application.

## License

MIT