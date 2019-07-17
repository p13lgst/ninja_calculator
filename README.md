# Ninja Calculator

This app is a calculator created using [Svelte](https://svelte.dev)
The parsing of and evaluation of expressions are made using the [mathjs](https://mathjs.org/) library

## Live Demo

A live demo of this app is hosted at: [ninjacalculator.surge.sh](https://ninjacalculator.surge.sh)

## TODOS

- [ ] Add keyboard with:
  - [ ] Numbers
  - [ ] Operators
  - [ ] Functions
- [ ] Add an option to disable imaginary numbers
- [ ] Add a way to create and use custom functions
- [ ] Replacer '*' with a better multiplication operator
- [ ] Add support for symbolic mathematics
- [ ] Integrate a Latex Editor for easier usability of functions
- [ ] Generate graphic of functions

## Running locally

Open a terminal and run the following to run the app locally

### Downloading the source code

```bash
git clone https://github.com/p13lgst/ninja_calculator.git
cd ninja_calculator
```

### Installing dependencies

If you have yarn installed:

```bash
yarn install
```

Otherwise:

```bash
npm install
```

### Launching development server

```bash
yarn run dev
```

or:

```bash
npm run dev
```

### Building a production version

```bash
yarn run build
```

or:

```bash
npm run build
```
