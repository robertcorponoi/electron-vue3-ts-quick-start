<p align="center">
  <img width="250" height="250" src="https://github.com/robertcorponoi/graphics/blob/master/electron-vue3-ts-quick-start/logo/logo.png?raw=true">
</p>

<h1 align="center">Electron Vue3 Typescript Quick Start</h1>

<p align="center">Easy to use template for creating an app with Electron, Vue3, and Typescript<p>

This is a vue3 application created with the [vue-cli](https://cli.vuejs.org/) with Electron added on.

## **Table of Contents**

- [Features](#features)
- [Scripts](#scripts)

## **Features**

- [Vue3](https://v3.vuejs.org/)
- [Babel](https://babeljs.io/)
- [ESLint](https://eslint.org/)
- [Mocha](https://mochajs.org/) & [Chai](https://www.chaijs.com/) for testing.
- [Typescript](https://www.typescriptlang.org/) support for Vue components
- [electron-reloader](https://github.com/sindresorhus/electron-reloader) to reload the app on changes
- [electron-builder](https://github.com/electron-userland/electron-builder) for packaging and building your Electron app.
- [dotenv](https://github.com/motdotla/dotenv) to load environment variables

## **Scripts**

- `npm run start`: Starts the Electron app.
- `npm run build:dev`: Builds the Vue app to the `dist` directory which is used by Electron to display the app.
- `npm run build:dev:watch`: The same as above except it watches for and reloads on changes.
- `npm run build:prod`: Creates a production ready build.
- `npm run test:unit`: Runs the unit tests defined under `test/unit`.
- `npm run lint`: Runs ESLint to check for issues.
- `npm run dist`: Runs `npm run build:prod` and then calls electron-builder to package the Electron app.
- `npm run dist:mac`: Runs `npm run build:prod` and then calls electron-builder to package the Electron app for OSX.
- `npm run dist:linux`: Runs `npm run build:prod` and then calls electron-builder to package the Electron app for a Linux environment.
- `npm run dist:windows`: Runs `npm run build:prod` and then calls electron-builder to package the Electron app for Windows.
- `npm run dist:all`: Runs `npm run build:prod` and then calls electron-builder to package the Electron for OSX, Linux, and Windows.

## **Instructions**

1. Clone the repository
2. Run `npm install` to install the dependencies needed.

To develop, you need to follow the steps below every time you begin working on it:

1. First you want to run `npm run build:dev:watch` to build the `dist` directory and watch for changes to your Vue templates/components.
2. Run `npm run start` to start Electron.

Now, with both of these running, whenever you make a change to the files Electron uses or the Vue files, the Electron window will update automatically.

**Note:** The electron files are not Typescript so that they can be reloaded with electron-reloader.