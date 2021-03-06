# react-umd-loader-uni [![experimental](http://badges.github.io/stability-badges/dist/experimental.svg)](http://github.com/badges/stability-badges)

[![npm version](https://img.shields.io/npm/v/react-umd-loader-uni.svg)](http://npmjs.org/react-umd-loader-uni)

## Fork info

This is fork of [react-umd-loader](https://github.com/revolunet/react-umd-loader) which can also load ES6 React modules in UMD format.
This version supports React 16. For support of earlier versions of React, use version 1.x of this library.

## Original readme

Async load any remote [UMD](https://github.com/umdjs/umd) compatible React component into your app.

This component use [script.js](https://github.com/ded/script.js/) for loading the remote component.

See also : [React jspm loader](https://github.com/revolunet/react-jspm-loader)

## Usage

You can use [unpkg.com](unpkg.com) or whatever hosting. The only requirement is that the build supports [UMD](https://github.com/umdjs/umd).

This example loads the remote `react-json-viewer` component into our app

```js
import UmdLoader from 'react-umd-loader-uni'

let cmp = (<UmdLoader url="https://rawgit.com/coryhouse/my-component/master/umd/my-component.js" name="MyComponent" props={{ username: 'Person', message: 'you are here' }}>
             <p>Loading remote component...</p>
           </UmdLoader>);

```

As UMD exposes objects on `window`, you also need to define the name of the final module.


## Dev

This project use the great [react-component-boilerplate](https://github.com/survivejs/react-component-boilerplate)

