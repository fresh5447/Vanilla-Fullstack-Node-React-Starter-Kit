## About

Basic fullstack node react app that you can clone and get up and running without having to configure a client/server proxy, custom scripts to make life easy, create-react-app with less boilerplate code, a node server ready to build out an `express` app, and linting that works for the client and server.

---

### Install Dependencies

Scripts are setup to use `npm`, if you wish to use `yarn` simply replace `npm` with `yarn` in `package.json`, `client/package.json`, and `server/package.json`

1) `npm install`  *install dependencies at root level*

2) `npm run install:client && npm run install:server` *install node server and react app specific dependencies.*

----

### Fire up the app

1) `npm run start:db`  *starts up local mongo process, you can alternatively just try `sudo mongod` in the terminal.*

2) `npm run start:server` *start the node server*

3) `npm run start:client` *start the react app using react scripts*

__Tip__
You can run both the previous steps in one command:
`npm run install:client && npm run install:server`

_Browser is loaded at `localhost:3000` and server api is located at `localhost:3001`_

----


### Client

The client was basically bootstrapped with `create-react-app`, but was gutted to include less boilerplate code.
The `package.json` additionally includes a `proxy` which makes it play nice with your local `node` app.
The react app is also ready to rock for `jss`.

----

### Server
Basic `node` server with appropriapte dependencies isntalled to build out API with `express`.

There are also some basic testing utilties included in the initial install:
  - chai
  - mocha
  - chaihttp

----

### What Now

Be sure to update the line in `server/server.js` to use your local DB

`mongoose.connect('mongodb://localhost/__YOUR_DB__')`

----

### Eslint

Eslint is configured to lint `node` code under `server`, and `react` code under `client`. To modify the configuration head to `eslint.rc`

----

### Custom Scripts

There are a bunch of scripts to make your life easier, be sure to check em out in any of the `package.json`s!


