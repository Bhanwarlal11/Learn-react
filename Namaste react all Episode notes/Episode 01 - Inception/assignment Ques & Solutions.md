# Chapter 01 - Inception

## `Theory Questions :`

- What is `Emmet`?

- Difference between a `Library and Framework``

- What is `CDN`? Why do we use it?

- Why is `React` known as `React`?

- What is `crossorigin` in the script tag?

- What is the difference between `React and ReactDOM`?

- Difference between `react.development.js` and `react.production.js` files via CDN

- What is `async and defer`?

## `Coding Questions: `

Set Up Tools

- Create a `New Git Repo`

- Build Your First `Hello World` Program

- Create an Element

- Create `Nested React Elements`

- Use `root.render`

- Push Code to Github

- Prepare for Next Class

- Familiarize yourself with Arrow Functions.
- References:

  - [React `createElement` API](https://react.dev/reference/react/createElement)
  - [Introduction to Arrow Functions](https://www.youtube.com/watch?v=IrHmpdORLu8)

## 🔽⏬
## ⬇️⏬
## 🔽⏬
## ⬇️⏬

# `Theory assignment solution :`



## What is `Emmet`?

- Emmet is a powerful toolkit that enables efficient HTML and CSS coding. It provides a shorthand syntax to quickly expand code snippets, making it useful for creating complex structures.
- In Visual Studio Code (VS Code), Emmet is built-in and can be accessed by typing abbreviations and then pressing the Tab key to expand them.
- For example, typing `"div.container"` and pressing Tab will expand to:

```<div class="container"></div> ```



## Difference between a `Library and Framework`

- **library** is a collection of pre-written code that developers can use to perform specific tasks. A **framework**, on the other hand, provides a broader structure and guidelines for building applications. While libraries offer more flexibility, frameworks impose a specific architecture.
- One key difference between libraries and frameworks is that libraries are called by the code, while frameworks call the code. In other words, when you use a library,you are in control of how and when it is used. With a framework, the framework is in control and dictates how the code should be organized and used.



## What is `CDN`? Why do we use it?

- **CDN (Content Delivery Network)** is a network of distributed servers that deliver web content to users based on their geographical location. CDNs improve page load times and reduce server load by caching content closer to users, resulting in a faster and more reliable browsing experience.



## Why is `React` known as React?

- React, often referred to as **React.js**, gets its name from its core concept of "reactive" user interfaces. It allows developers to build dynamic and interactive UI components that react to changes in data, providing a smoother user experience.
- Facebook and an open-source developer community run it.


-

## What is `crossorigin` in the script tag?

- The `crossorigin` attribute in a script tag is used to specify how the browser should handle requests for cross-origin scripts. It helps prevent security vulnerabilities by controlling how external resources are accessed and used in your web application.
- The purpose of crossorigin attribute is used to share the resources from one domain to another domain. Basically, it is used to handle the CORS request. It is used to handle the CORS request that checks whether it is safe to allow for sharing the resources from other domains.
- The crossorigin attribute on a `<script>` tag specifies that CORS is supported when loading an external script file from a third party server or domain. 
- CORS is a standard mechanism used to retrieve files from other domains.

```<script crossorigin="anonymous|use-credentials">```



## Difference between `React and ReactDOM`

- React and ReactDOM are two separate libraries that are often used together in the development of web applications with React.
- **React** is a JavaScript library for building user interfaces, while **ReactDOM** is a package that specifically deals with rendering React components into the DOM (Document Object Model).
ReactDOM, on the other hand, is a library that provides an interface between React and the DOM (Document Object Model). The DOM is a tree-like structure that
represents the HTML of a web page, and ReactDOM provides a set of functions that allow React components to be rendered to the DOM and updated efficiently.
The react package contains React.createElement() , React.Component , React.Children , and other helpers related to elements and component classes. You can think of
these as the isomorphic or universal helpers that you need to build components.The react-dom package contains ReactDOM.render() , and in react-dom/server we
have server-side rendering support with ReactDOMServer.renderToString() and ReactDOMServer.renderToStaticMarkup() .

const listElement = React.createElement( 'li', {
className: 'list'
}, 'React.js' );

ReactDOM.render( listElement, document.querySelector( '#root' ) );

*
*
*
*
*
*
*





## Difference between `react.development.js` and `react.production.js` files via CDN

The `react.development.js` file provides a larger file size with additional development-friendly features like debugging messages. The `react.production.js` file, on the other hand, is optimized for production environments, resulting in a smaller file size and improved performance.
Development JS for development reasons. You have Source Maps, debugging and often times hot reloading ability in those builds.
The production build, on the other hand, runs in production mode which means this is the code running on your client’s machine.

*
*
*
*
*
*



## What is `async and defer`?

The `async` and `defer` attributes in the script tag control how scripts are loaded and executed on a web page. 
**Async** loads the script asynchronously without blocking the rendering of the page.
<script async src="script.js"></script>

**Defer** also loads the script asynchronously but ensures the script is executed in the order they appear in the HTML document after the page is fully parsed.

<script defer src="script.js"></script>
