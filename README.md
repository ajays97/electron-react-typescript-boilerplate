## Electron-React Boilerplate with TypeScript

Note: If you are using Windows, chances are you’ll face an error, this is because NODE_ENV is not recognized as a command. You have to install crossenv and place the command before NODE_ENV.

```
npm install --save-dev cross-env
```

### On Windows, use `cross-env` before script

For example,

```
"scripts": {
    "dev:electron": "cross-env NODE_ENV=development webpack --config webpack.electron.config.js --mode development && electron .",
    "dev:react": "cross-env NODE_ENV=development webpack-dev-server --config webpack.react.config.js --mode development"
  },
```

To run this project.

- Clone this repo

```bash
  git clone https://github.com/elisealcala/electron-react-ts.git
```

- Install the dependencies

```bash
  npm install
```

- Now run these two commands in separate consoles.

```bash
  npm run dev:react
```

```bash
  npm run dev:electron
```
