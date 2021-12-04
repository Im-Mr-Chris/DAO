

Template to help you build your first Aragon application following the [tutorial from hack.aragon](https://hack.aragon.org/docs/tutorial.html)

## Running your app

To run the app in a browser with front end plus back end hot reloading, simply run `npm start`.

## What's in this boilerplate?

### npm Scripts

- **postinstall**: Runs after installing dependencies.
- **build-app**: Installs front end project (app/) dependencies.
- **start** Runs your app inside a DAO.
- **compile**: Compiles the smart contracts.

### Structure

This boilerplate has the following structure:

```md
root
├── app
├ ├── src
├ ├ ├── App.js
├ ├ ├── index.js
├ ├ └── script.js
├ └── package.json
├── contracts
├ └── CounterApp.sol
├── scripts
├ └── buidler-hooks.js
├── arapp.json
├── manifest.json
├── buidler.config.js
└── package.json
```

- **app**: Frontend folder. Completely encapsulated, has its package.json and dependencies.
  - **src**: Source files.
    - `App.js`: Aragon app root component.
    - `index.js`: Aragon app entry point.
    - `script.sol`: Aragon app background script.
  - [**package.json**](https://docs.npmjs.com/creating-a-package-json-file): Frontend npm configuration file.
- **contracts**: Smart Constracts folder.
  - `CounterApp.sol`: Aragon app contract.
- **scripts**: Scripts folder.
  - `buidler-hooks.js`: Buidler script hook.
- **test**: Tests folder.
- [**arapp.json**](https://hack.aragon.org/docs/cli-global-confg#the-arappjson-file): Aragon configuration file. Includes Aragon-specific metadata for your app.
- [**manifest.json**](https://hack.aragon.org/docs/cli-global-confg#the-manifestjson-file): Aragon configuration file. Includes web-specific configurations.
- [**buidler.config.js**](https://buidler.dev/config/): Buidler configuration file.
- [**package.json**](https://docs.npmjs.com/creating-a-package-json-file): Main npm configuration file.

### Libraries

- [**@aragon/os**](https://github.com/aragon/aragonos): Aragon interfaces.
- [**@aragon/api**](https://github.com/aragon/aragon.js/tree/master/packages/aragon-api): Wrapper for Aragon application RPC.
- [**@aragon/ui**](https://github.com/aragon/aragon-ui): Aragon UI components (in React).
- [**@aragon/buidler-aragon**](https://github.com/aragon/buidler-aragon): Aragon Buidler plugin.
