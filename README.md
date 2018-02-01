# Up and running
Scripts are setup to use `npm`, if you wish to use `yarn` simply replace `npm` with `yarn` in `package.json`, `client/package.json`, and `server/package.json`

1) `npm install`  // install dependencies at root level.

2) `npm run install:client && npm run install:server` // install node server and react app specific dependencies.

# Fire up the app
1) `npm run start:db`  // starts up mongo process, you can alternatively just try `sudo mongod` in the terminal.

2) `npm run start:server` // start the node server

3) `npm run start:client` // start the react app using react scripts

Browser is loaded at `localhost:3000` and server api is located at `localhost:3001`

__Tip__
You can run both the previous steps in one command:
`npm run install:client && npm run install:server`

# What Now

Be sure to update the line in `server/server.js` to use your local DB
`mongoose.connect('mongodb://localhost/__YOUR_DB__')`

## Eslint

Eslint is configured to lint `node` code under `server`, and `react` code under `client`. To modify the configuration head to `eslint.rc`

## Custom Scripts

There are a bunch of scripts to make your life easier, be sure to check em out!


