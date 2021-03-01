# ≧(´▽ ｀)≦ Angular Universal Pre-Render

This project will guide you through the process of pre-rendering your Angular project using [Angular Universal](https://angular.io/guide/universal) and deploy it to a CDN with with [Netlify](https://www.netlify.com/?_ga=2.14078323.599079780.1612319207-1714706019.1588285059?utm_source=repo&utm_medium=au-pre-render-tzm&utm_campaign=devex).

> 📓 [Check out this blog post](https://hubs.ly/H0GZfCp0) to get even more details about what's going on in this project.

## Setup

To skip all this you could also just click this button:

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/tzmanics/angular-universal-pre-render&utm_source=github&utm_medium=ng-prerender-tzm&utm_campaign=devex)

### Local Setup

- install with `npm i`
- run `npm run prerender` to build and pre-render your app
- you can see all the built files in `dist/<project name>/browser
- to serve with Angular Universal locally run `ng serve:ssr`

### Productions Setup

- install the Netlify CLI `npm i netlify-cli -g`
- run `netlify init` to setup the project on Netlify & deploy it! (the [/netlify.toml](/netlify.toml) file has the information Netlify needs to deploy your app)
- run `netlify open` to open the project dashboard, under the 'Functions' tab you can find the endpoint for your function as well as see all the logs.u

## The pieces

- this project has a skeleton for an eCommerce application that can be used as an app shell that can pre-rendered and then hydrated with [Netlify Function](https://www.netlify.com/products/functions/?utm_source=repo&utm_medium=au-prerender-tzm&utm_campaign=devex).
- there are also files added to implement [Angular Universal](https://angular.io/guide/universal) so even though we are only using the pre-render functionalities of AU you are set up to take advantage of the whole SSR technology
- the only other additional file is the [Netlify configuration file](https://docs.netlify.com/configure-builds/file-based-configuration/?utm_source=repo&utm_medium=au-prerender-tzm&utm_campaign=devex) which tells Netlify how and what to deploy to the CDN :)

# Angular CLI Infos

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
