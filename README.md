# nuxt-netlify-functions-example

[![Netlify Status](https://api.netlify.com/api/v1/badges/ae375e95-eb24-46ed-95d3-a8591add95bc/deploy-status)](https://app.netlify.com/sites/nuxt-netlify-functions-example/deploys)
[![GitHub Actions](https://img.shields.io/github/workflow/status/wearelucid/nuxt-netlify-functions-example/End-to-end%20tests?label=build&logo=github&style=for-the-badge)](https://github.com/wearelucid/nuxt-netlify-functions-example)

> Nuxt.js example for running Netlify functions locally in a dev environment and as a generated static site deployed to Netlify.

> Heavily inspired by the [official guide](https://functions-playground.netlify.com/) and [this example](https://github.com/stefanjudis/service-party).

## Demo

Live demo can be found [here](https://nuxt-netlify-functions-example.netlify.com/).

## Testing functions locally

Thanks to the [Netlify Dev](https://www.netlify.com/products/dev/) command in the Netlify CLI (`yarn global add netlify-cli`), you can test your functions locally with no build step involved!

After building the app and running `netlify dev` or `ntl dev`, you can test the functions locally by hitting the endpoint http://localhost:8888/.netlify/functions/<function-name>

## Build Setup

```bash
# Use Node version specified in nvmrc
$ nvm use

# Install dependencies
$ yarn

# Serve Nuxt app and Netlify functions at localhost:8888
$ netlify dev

# Generate static project
$ yarn generate
```

## Running Tests

Tests use the Netlify CLI to run the serverless functions locally. You'll probably be prompted to login with your Netlify account.

```bash
# Serve Nuxt app and Netlify functions at localhost:8888
$ netlify dev

# Run this command in another terminal
$ yarn test
```
