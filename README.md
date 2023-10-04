# Basic React Starter Library

This is a basic React library template with TypeScript. It's a starting point for building reusable React components and sharing them as a library.

## Features

- React components
- TypeScript for type checking
- Rollup for bundling
- Storybook for component development and documentation
- Jest for testing
- Eslint and Prettier for code linting and formatting

## Installation

To use this library in your project, you can install it via npm or yarn:

```bash
npm install
# or
yarn add my-react-library
```

## Publishing the library
```package.json```
```
{
  "name": "@YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME",
  "publishConfig": {
    "registry": "https://npm.pkg.github.com/YOUR_GITHUB_USERNAME"
  },
  ...  
}
```
```~/.npmrc```
```registry=https://registry.npmjs.org/
@YOUR_GITHUB_USERNAME:registry=https://npm.pkg.github.com/
//npm.pkg.github.com/:_authToken=YOUR_AUTH_TOKEN
```

You can get your github authentication token from [here](https://github.com/settings/tokens)


## Usage

Running storybook instance
```
npm run storybook
```

Running rollup
```
npm run rollup
```

Pulishing your library to npm (after initialization)

```
npm publish
```

Run tests using Jest

```
npm run test
```

### Usage of library in a project

Installing the library 

```
npm install @YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME
```


Importing the library
```
import React from 'react';
import { button as Button } from '@YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME';
```

Using the imported component 

```
function App() {
  return (
    <div className="App">
      <Button label='Hello World!' />
    </div>
  );
}

export default App;
```
