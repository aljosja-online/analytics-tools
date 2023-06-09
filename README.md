# analytics-tools

> This readme is automatically generated by [create-ink-app](https://github.com/vadimdemedes/create-ink-app)

## Install

```bash
$ npm install --global analytics-tools
```

## CLI

```
$ analytics-tools --help

  Usage
    $ analytics-tools

  Options
    --name  Your name

  Examples
    $ analytics-tools --name=Jane
    Hello, Jane
```

Here's a brief overview of each file:

1. `source/app.tsx`: This file defines a React component named `App`, which takes a single prop `name` and renders "Hello, " followed by the name in green. If `name` is not provided, it defaults to "Stranger".

2. `source/cli.tsx`: This file is the entry point for your command-line application. It uses the `meow` library to parse command-line arguments and define flags. In this case, you have a `name` flag of type `string`. The `render()` function from Ink is used to render the `App` component with the `name` prop set to the value of the `name` flag provided by the user.

3. `package.json`: This file contains the metadata of your project, such as the name, version, dependencies, devDependencies, and various scripts for building and testing the application.

In order to run your application, you need to follow these steps:

1. Install the dependencies by running `npm install` or `yarn` in your project's root directory.

2. Build the TypeScript files by running `npm run build` or `yarn build`. This will compile your TypeScript files into the `dist` directory.

3. Run your CLI by running `node dist/cli.js` followed by any options you want to pass, for example: `node dist/cli.js --name=John`.

4. To make the CLI executable globally, you can either symlink the `dist/cli.js` file to a directory in your `PATH` or publish your package to npm and install it globally.