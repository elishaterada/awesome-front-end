# Awesome Front-End JavaScript
A list of awesome front-end  JavaScript libraries that help you build fast, scalable, and accessible web apps. The list contains the ones that I've used in production environment and are still relevant as of last time this repo was updated.

## Design

### [Emotion](https://emotion.sh/)

> Emotion is a library designed for writing css styles with JavaScript.

I've been a big fan of CSS-in-JS technique to bring the power of JS logic in my style composition. By importing styles as a module, you are creating more explicit style architecture that is smarter than referencing CSS class via string.

### [d3](https://www.npmjs.com/package/d3)

> D3 (or D3.js) is a JavaScript library for visualizing data using web standards. D3 helps you bring data to life using SVG, Canvas and HTML. D3 combines powerful visualization and interaction techniques with a data-driven approach to DOM manipulation, giving you the full capabilities of modern browsers and the freedom to design the right visual interface for your data.
  
The best data visualization library out there that can be used natively within any front-end eco-system including React. Use it without a wrapper and you’ll be able to utilize this library to it's full potential.

### [Greensock](https://www.npmjs.com/package/gsap)

> Ultra high-performance, professional-grade animation for the modern web

Greensock is hands-down the best JavaScript animation library out there. They have a paid plugins which is worth the price if you are looking to achieve morphing and stroke animation.

### [color](https://www.npmjs.com/package/color)

> JavaScript library for immutable color conversion and manipulation with support for CSS color strings.

If you already use CSS-in-JS in your project, why not bring smart color conversion utility into your project? This is a very straightforward library that provides functions you've probably used in the past with LESS/SCSS.

## Network

### [axios](https://www.npmjs.com/package/axios)

> Promise based HTTP client for the browser and node.js

While you can make REST API calls with native fetch or with similar libraries, axios provides a built-in HTTP request cancellation. So when your user types strings in autocomplete form field, you can guarantee to show the latest result from a server, vs whichever request resolved the last.

### [debounce-promise](https://www.npmjs.com/package/debounce-promise)

> Create a debounced version of a promise returning function

While cancelling request solves the problem of showing responses in wrong order, your app may still be pounding on a server with many requests. By debouncing promises, you can send minimal amount of requests to a server.

### [jsonp](https://www.npmjs.com/package/jsonp)

> A simple JSONP implementation.

There will be times when you need to work with a server that expects JSONP, and unfortunately axios does not cover it.

### [qs](https://www.npmjs.com/package/qs)

> A querystring parsing and stringifying library with some added security.

Depending on the API server you are working with, you might need to format query strings in particular way. Instead of writing your query string transformers, let qs take care of you.

### [koa](https://www.npmjs.com/package/koa)

> Expressive HTTP middleware framework for node.js to make web applications and APIs more enjoyable to write.

Why a server framework in this list? It's because of the SSR which enables Front-End engineers to generate server-side rendered results. You can definitely start with Express as a starter and learn to use more modular koa as you progress.

## Geojson

### [Turf.js](http://turfjs.org/)

> Modular, simple-to-understand JavaScript functions that speak GeoJSON

Turf.js is a collection of modules that help you work with GeoJSON data. The earth is not linear and you'll want modules to take care of calculating bounding box, distance, etc.

## Search

### [fuse.js](https://fusejs.io/)

> Lightweight fuzzy-search library. Zero dependencies.

There will be times you want to provide a fast and fuzzy-matching search results vs requesting data from server. For example, you may ask your user input for country, state, timezone, etc which is going to be more user-friendly to be able to search vs scroll.

## Textarea

### [linkifyjs](https://www.npmjs.com/package/linkifyjs)

> Linkify is a small yet comprehensive JavaScript plugin for finding URLs in plain-text and converting them to HTML links. It works with all valid URLs and email addresses.

Often it's user-friendly to turn their textarea input (e.g. description field) into a smart output with URLs converted into a link. Be sure to add `rel="noopener noreferrer"` if you are going to use it with `target="_blank"` for security reason.

## Date Time

### [luxon](https://moment.github.io/luxon/)

> A powerful, modern, and friendly wrapper for Javascript dates and times.

Luxon is a light-weight cousin of moment.js with added bonus of immutability. This is generally all you need to do date related operations.

### [moment-timezone](https://momentjs.com/timezone/)

> Parse and display dates in any timezone.

If you need to create a timezone modules with accurate time offsets, you'll want to generate them dynamically. Unfortunately, Luxon does not provide a data set so you'll need to use this library in conjunction.

## Gesture

### [Hammer.js](https://hammerjs.github.io/)

> Add touch gestures to your webapp.

If you worked hard to optimize your web app for mobile screens, you might as well provide handy gestures that some users might expect (e.g. swipe to move between tabs). Hammer.js provides a simple way to let you run functions based on gestures.

## Utilities

### [lodash](https://lodash.com/)

> A modern JavaScript utility library delivering modularity, performance & extras.

While ES6 brought many handy methods at our disposal, lodash still has loads of useful methods we'll be able to leverage and save time.

### [uniqid](https://www.npmjs.com/package/uniqid)

> A Unique Hexatridecimal ID generator.

When you need to work with an array of objects (e.g. list of user entered emails), that does not have unique ID, you can use this library vs using index.

### [git-rev-sync](https://www.npmjs.com/package/git-rev-sync)

> Synchronously get the current git commit hash, tag, count, branch or commit message. Forked from git-rev.

This library is useful when you want to tag your build with commit hash vs timestamp of build (locally or in CI env).

## React

### [mobx](https://mobx.js.org/)

> Simple, scalable state management

Mobx is simple, and that is beneficial for working with peer coders or for your own sanity.

### [next](https://nextjs.org/)

> Production grade React applications that scale. The world’s leading companies have used Next.js to build server-rendered applications, static websites, and more.

If you want to create React based app that is built for SSR, go with Next.js. Once you learn the basics, you'll feel great about putting minimal effort to gain benefit of automatic code-splitting, SEO benefits, initial bundle size, etc.

### [react-scroll](https://www.npmjs.com/package/react-scroll)

> Component for animating vertical scrolling.
  
If you need to trigger a scroll within a container (vs global scroll bar), this will come in handy.

### [react-copy-to-clipboard](https://www.npmjs.com/package/react-copy-to-clipboard)

> Copy to clipboard React component

If you need a share button that copies the URL into users' clipboard, this library will help you do exactly that.

### [react-truncate](https://www.npmjs.com/package/react-truncate)

A handy library that can truncate text

### [react-countup](https://www.npmjs.com/package/react-countup)

> A configurable React component wrapper around CountUp.js.
  
Spice up your dashboard numbers with this library that can gradually count up and down the numbers

### [react-modal](https://www.npmjs.com/package/react-modal)

> Accessible modal dialog component for React.JS

The simple to use accessible modal for React, a no-brainer choice.

### [react-onclickoutside](https://www.npmjs.com/package/react-onclickoutside)

> This is a React Higher Order Component (HOC) that you can use with your own React components if you want to have them listen for clicks that occur somewhere in the document, outside of the element itself (for instance, if you need to hide a menu when people click anywhere else on your page).

A handy HoC that help trigger close on flyout components you build.  

### [react-day-picker](https://github.com/gpbl/react-day-picker)

> Flexible date picker for React

This is a flexible and accessible date picker for React.
