# Jest Getting Started

## About

Code along of Jest's [Getting Started](https://jestjs.io/docs/getting-started) tutorial.

## Notes

### Jest Setup Workflow

0. `cd` into our GitHub repo or project directory.

1. Run:

```
npm init -y
```

2. Run:

```
npm install --save-dev jest
```

3. Add the following section in the `package.json`:

```
{
  "scripts": {
    "test": "jest"
  }
}
```

#### ES6 Modules

*If* we wish to use ES6 modules, and do not want to use [Babel](https://babeljs.io/), then do the following:

> Steps `0`, `1`, `2` are same as previous.

0. `cd` into our GitHub repo or project directory.

1. Run:

```
npm init -y
```

2. Run:

```
npm install --save-dev jest
```

3. Add the following sections in the `package.json`:

```
"type": "module",
"jest": {
    "transform": {}
},
"scripts": {
    "test": "node --experimental-vm-modules node_modules/jest/bin/jest.js"
},
```

**Source**: <https://stackoverflow.com/questions/35756479/does-jest-support-es6-import-export>

## Background

This was done as part of [The Odin Project](https://www.theodinproject.com/)'s assignment from the lesson [Testing Basics](https://www.theodinproject.com/lessons/node-path-javascript-testing-basics):

> Follow along to [Jest’s Getting Started tutorial](https://jestjs.io/docs/getting-started). For the upcoming testing practice and project, you only need to follow the instructions for installing jest.