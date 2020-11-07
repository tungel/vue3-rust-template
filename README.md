# vue3-rust-template

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your unit tests
```
npm run test:unit
```

### Run your end-to-end tests
```
npm run test:e2e
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## For reference, steps to recreate from scratch

```
npm install --global @vue/cli


# 2. Create a new project, then choose the "Manually select features" option
# then select:
# - Choose Vue version
# - TypeScript
# - Router
# - Linter / Formatter
# - Unit Testing
# - E2E Testing
# then, select Vue version `3.x (Preview)`
vue create vue3-rust-template
```

The options I selected:

```
Vue CLI v4.5.8
? Please pick a preset: Manually select features
? Check the features needed for your project: Choose Vue version, TS, Router, Linter, Unit, E2E
? Choose a version of Vue.js that you want to start the project with 3.x (Preview)
? Use class-style component syntax? Yes
? Use Babel alongside TypeScript (required for modern mode, auto-detected polyfills, transpiling JSX)? Yes
? Use history mode for router? (Requires proper server setup for index fallback in production) Yes
? Pick a linter / formatter config: Standard
? Pick additional lint features: Lint on save
? Pick a unit testing solution: Mocha
? Pick an E2E testing solution: Cypress
? Where do you prefer placing config for Babel, ESLint, etc.? In dedicated config files
? Save this as a preset for future projects? Yes
```

Next:

```
npm install --save-dev wasm-tool/wasm-pack-plugin
npm install --save text-encoding
```

## Ref

- https://v3.vuejs.org/guide/typescript-support.html#recommended-configuration
