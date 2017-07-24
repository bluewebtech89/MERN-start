# mern-starter
[![Build Status](https://travis-ci.org/ming-soon/mern-starter.svg?branch=master)](https://travis-ci.org/ming-soon/mern-starter)

MERN (MongoDB, Express, React, Node)

MERN is your One-Stop solution which makes it easy to build universal apps. It minimizes the setup time and gets you up to speed using proven technologies and best practices.

## Features
- [**Universal**](http://isomorphic.net/) App
- ES2015 features and JSX syntax with [**Babel**](https://babeljs.io/).
- Server-side rendering with [**React Router**](https://github.com/ReactTraining/react-router) 3.x.
- [**Redux**](http://redux.js.org/) predictable state containers.
- [**Redux Saga**](https://redux-saga.github.io/redux-saga/) [~~Redux Thunk~~](https://github.com/gaearon/redux-thunk) for asynchronous action creators.
- Hot reloading using [**Webpack HMR**](https://webpack.js.org/concepts/hot-module-replacement/).
- [**Webpack 2**](https://webpack.js.org/) for both development and production bundles.
- [**CSS Modules**](http://glenmaddern.com/articles/css-modules) allows for modular and reusable CSS.
- Responsive front-end interface with [**Bootstrap 3**](http://getbootstrap.com/).
- [**Express**](http://expressjs.com/) 4.x server.
- [**Mongoose**](http://mongoosejs.com/) for MongoDB.
- Server-side authentication with [**Passport**](http://passportjs.org/).
- Linting with [**Eslint**](http://eslint.org/) and [**Airbnb**](https://github.com/airbnb/javascript) JavaScript Style Guide.
- Unit testing with [**Mocha**](https://mochajs.org/), [**Enzyme**](http://airbnb.io/enzyme/) and [**SuperTest**](https://github.com/visionmedia/supertest).

## Quickstart
```
git clone https://github.com/ming-soon/mern-starter.git your_app
cd your_app
npm install
npm run start
```
**Note: Please make sure your MongoDB is running.**

## Available Commands
1. `npm run start` - starts the production server.

2. `npm run start:dev` - starts the development server with hot reloading enabled.

3. `npm run test` - starts the test runner.

4. `npm run eslint:src` - runs linter to check for lint errors.

## File Structure
### Webpack Configs
MERN users Webpack for bundling modules. There are three types of Webpack configs provided `webpack.base.config.js` (for base configuration), `webpack.app.config.js` (for bundling app), , `webpack.config.server.js` (for bundling server in production).

Webpack is configured to make use of `resolve.alias`, which lets you create aliases to `import` or `require` certain modules more easily.

### Server
MERN uses Express framework.

If `NODE_ENV` is development, we apply Webpack middlewares for bundling and Hot Module Replacement.

### Client
The `app` directory contains all the shared components, routes and reducers.

### Configuration
The `configs` directory contains all configuration settings.

Default project configuration can be found in `~/config/project.config.js`.

The `.scss` file extension is supported out of the box. After being imported, styles will be processed with PostCSS for autoprefixing, and will be extracted to a `.css` file during production builds.

### Test
The `test` directory contains unit test cases.

## License
MERN is released under the [MIT License](https://opensource.org/licenses/MIT)
