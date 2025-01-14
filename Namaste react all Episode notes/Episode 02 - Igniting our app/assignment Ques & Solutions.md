# Chapter 02 - Igniting our app

## `Theory Questions :`

- What is `NPM`?

- What is `Parcel/Webpack`? Why do we need it?

- What is `.parcel-cache`?

- What is `npx` ?

- What is `difference` between `dependencies` vs `devDependencies`

- What is `Tree Shaking`?

- What is `Hot Module Replacement`?

- List down your `favorite 5 superpowers of Parcel` and `describe any 3` of them in your
  own words.

- What is `.gitignore`? What should `we add` and `not add` into it?

- What is the `difference` between `package.json` and `package-lock.json`

- Why should I not modify `package-lock.json`?

- What is `node_modules` ? Is it a `good idea to push that on git`?

- What is the `dist` folder?

- What is `browserlists`

- Read about `dif bundlers`: `vite`, `webpack`, `parcel`

- Read about: `^` - `caret` and `~` - `tilde`

- Read about `Script types in html` (MDN Docs)

## Installation tasks:

- In your `existing project`
- initialize `npm` into your `repo`

  - install `react` and `react-dom`

  - `remove CDN` links of `react`

  - `install parcel`

  - `ignite your app` with parcel

  - add scripts for `“start”` and `“build”` with `parcel commands`

  - add `.gitignore` file

  - add `browserlists`

  - `build a production version` of your code using `parcel build`

- References:

- [Creating your own create-react-app](https://medium.com/@JedaiSaboteur/creating-a-react-app-from-scratch-f3c693b84658)
- [Parcel Documentation](https://parceljs.org/getting-started/webapp/)
- [Parcel on Production](https://parceljs.org/features/production/)
- [BrowsersList](https://browserslist.dev/)

## ⬇️⤵️

## ⏬🔽

## ⬇️⤵️

## ⏬🔽

# `Theory assignment solution :`

## What is `NPM` ?

- It is a tool used for package management and the default package manager for Node projects. NPM is installed when NodeJS is installed on a machine.
- It comes with a command-line interface (CLI) used to interact with the online database of NPM. This database is called the NPM Registry, and it hosts public and private
- 'packages.' To add or update packages, we use the NPM CLI to interact with this database.
- We use NPM because we want a lot of packages in our Projects/React App.
- `**Note :**` npm does not stand for node package manager but everything else. `Node package manager is not a full form of NPM` (It stands for anything but not a abbreviation for node package manager)
- `npm` alternative is `yarn`
- `How to initialize npm ?`
- `npm init`
- `npm init -y` can be used to skip the setup step, npm takes care of it and creates the `package.json` json file automatically , but without configurations.

## What is `Parcel/Webpack`? Why do we need it?

- `parcel`: Parcel is a tool that helps web developers bundle all the different files and code for a website or app together in a way that makes it faster to load and run. It's really easy to set up and works well for simple projects.

- `Webpack`: Webpack is another tool that does a similar job but gives developers more control over how things are bundled. It's more powerful and flexible, which makes it a good choice for complex projects where customization is important.
- `Parcel and webpack` are the bundlers used mostly for JavaScript or Typescript code that helps you to minify, clean, and make your code compact so that it becomes easier to send a request or receive the response from the server when it usually takes you to transfer multiple files without using any bundler for loading the page of your application.

**Parcel Features:**

- `HMR (Hot Module Replacement):` Enables real-time changes to your code without needing to refresh the entire page, making development faster and more efficient.
- `File watcher algorithm in C++:` A performant file watcher that efficiently tracks changes to your code and rebuilds only what's necessary.
- Bundling: Combines all of your code and dependencies into a single file, making it easier to deploy and reducing page load times.
- `Code minification:` Reduces the size of your code by removing unnecessary whitespace and renaming variables, making it faster to download and execute.
- `Image optimization:` Automatically optimizes images to reduce their size without sacrificing quality, improving page load times.
- `Caching:` Speeds up development by caching assets and only rebuilding when necessary, improving build times.
- `Compression:` Reduces the size of your assets, making them faster to download and improving page load times.
- `Tree shaking:` Tree shaking is a technique used in JavaScript module bundlers, such as Webpack or Parcel, to eliminate unused code from the final bundled output. It helps optimize the bundle size by removing dead or unreachable code.

**installation commands:**
`npm install -D parcel`

- `D` is used for development and as a development dependency.

_Parcel Commands :_

- For development build:
  `npx parcel <entry_point>`
- For production build :
  `npx parcel build <entry_point>`

## What is `.parcel-cache`?

`.parcel-cache` is used by parcel(bundler) to reduce the building time. It stores information about your project when parcel builds it, so that when it rebuilds, it doesn't have to re-parse and re-analyze everything from scratch. It's a key reason why parcel can be so fast in development mode.

- The dist folder contains the output of Parcel and the content of that folder is served by the web server.

## What is `npx` ?

`npx` is a tool that is used to execute the packages. It comes with the npm, when you installed npm above 5.2.0 version then automatically npx will installed. It is an npm package runner that can execute any package that you want from the npm registry without even installing that package.

## What is `difference` between `dependencies` vs `devDependencies`

- `Dependencies` should contain library and framework in which your app is built on, needs to function effectively. such as `Vue`, `React`, `Angular`, `Express`, `JQuery` and etc.
- `DevDependencies` should contain modules/packages a developer needs during development. such as, `parcel`, `webpack`, `vite`, `mocha`. These packages are necessary only need while you are developing your project, not necessary on production.

## What is `Tree Shaking`?

`Tree shaking` is process of removing the unwanted code that we do not use while developing the application. In computing, tree shaking is a dead code elimination technique that is applied when optimizing code.

## What is `Hot Module Replacement`?

`HMR` is designed to make the development process smoother and more efficient by allowing you to see changes in your code immediately without having to manually refresh the entire page.

## List down your `favorite 5 superpowers of Parcel` and `describe any 3` of them in your own words.

`superpowers of parcel`:

- `HMR (Hot module replacement)` - parcel allows to see changes in the code immediately without having to manually refresh the entire page.
- `Diagnostic` - parcel make errors looks beautiful with some color and it indicates the exact line where the error is occured.
- `Tree shaking` - parcel removes the unwanted code(dead code) that we do not use while developing the application.
- `Image optimization`
- `Differential bundling`

## What is `.gitignore`? What should `we add` and `not add` into it?

`gitignore` is a text file that holds which files or folders needs to be ignored in a project during commit to the repository. any files or folder that can be regenerated in our app needa to be added in the `gitignore` file, `package.json` and `package-lock.json` files should not be included in the gitignore file.

The entries in this file can also follow a matching pattern.

```
* is used as a wildcard match
/ is used to ignore pathnames relative to the .gitignore file
# is used to add comments to a .gitignore file
```

This is an example of what the .gitignore file could look like:

```
# Ignore Mac system files
.DS_store

# Ignore node_modules folder
node_modules

# Ignore all text files
*.txt

# Ignore files related to API keys
.env

# Ignore SASS config files
.sass-cache
```

## What is the `difference` between `package.json` and `package-lock.json`

- `package.json` : file constains the basic information of the project in JSON format, for ex: name, author, version, description etc..

- `package-lock.json` : file maintains all the version of the data which has been upgrated and It records the same version of the installed packages which allows to reinstall them. Future installs will be capable of building identical description tree.

## Why should I not modify `package-lock.json`?

The file contains the information about the dependencies and their versions used in the project. Deleting it would cause dependencies issues in the production environment. So don't modify it, It's being handled automatically by NPM.

## What is `node_modules` ? Is it a `good idea to push that on git`?

When you run npm install they are downloaded from the web and copied into the node_modules folder and Nodejs is trained to look for them there when you import them (without a specific path). `Don't push node_modules` in github because it contains lots of files(more than 100 MB), it will cost you memory space.

## What is the `dist` folder?

The `/dist` folder contains the minimized version of the source code. The code present in the `/dist` folder is actually the code which is used on production web applications. Along with the minified code, the `/dist` folder also comprises of all the compiled modules that may or may not be used with other systems.

## What is `browserlists`?

`Browserlist `is a tool that allows to us tell react that what are the browser that our project/app should support, for that we need to modify `package.json`.

`Ex`:

In the package.json we need to modify like below:

```
"browserslist" : [
    "last 2 version"
]
```

- PS : it always good to mention like `"last 2 version" `so it will support all the browsers for the last 2 versions
