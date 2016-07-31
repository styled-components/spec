# CSS Components Spec

[![Join the chat at https://gitter.im/css-components/spec](https://badges.gitter.im/css-components/spec.svg)](https://gitter.im/css-components/spec?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Design Requirements and Spec for a Component-oriented CSS Solution

_**Note** the goal of this project at the moment is not to invent yet another CSS framework or library, but to discuss broader requirements and the state of the ecosystem as a whole - see [#6](https://github.com/css-components/spec/issues/6)_

---

## What is CSS Components?

Components are the new way of composing user interfaces for the web, whether they're implemented as template strings in [choo](https://github.com/yoshuawuyts/choo), Components in [Angular](https://angular.io) or Classes in [React](http://reactjs.com).

Components isolate the concerns of UI functionality and styling, so you can create small blocks of functionality that are easily designed, implemented and tested then compose a more complicated website or application from them without losing the simplicity.

While this challenges traditionally held beliefs about the separation of structure and style, and the technical separation of CSS and JavaScript, we believe it's the future. Read @chantastic's [blog post](https://medium.com/learnreact/scale-fud-and-style-components-c0ce87ec9772) for more background.

---

There are several competing solutions for how to effectively write and publish CSS with Components, including:

* CSS in JS (Aphrodite, JSS, etc.)
* Inline Styles (Radium, etc.)
* CSS Modules (+ postCSS, etc.)
* Traditional Stylesheets (+ LESS, SASS etc.)

At the moment the community is fragmented, and none of these solutions consistently solve all the concerns. 

The ideal solution would likely take inspiration from all of the above. See our [comparison](https://github.com/css-components/comparison) repo for a more comprehensive overview of the state of current solutions.

---

## Requirements

_**WIP** please discuss requirements in the issues!_

A complete CSS Components solution would include support for the following:

* work well for open source components that are themeable and not opinionated about build requirements (see [#3](https://github.com/css-components/spec/issues/3)
* has a good solution for overriding styles on child elements (see [#5](https://github.com/css-components/spec/issues/5)
* server side rendering
* don’t break inline styles
* fast at runtime (pre-buildable?)
* styles are colocated with components
* isolated as much as possible (styles == component)
* overridable and preferably not opinionated about how (we’re talking about CSS after all)
* supports css stuff like `:hover`, media queries (i.e. you shouldn’t be blocked from doing anything you can do with css)
* doesn’t create a bunch of wrapper components
* small and lightweight enough that you don't think twice about having it as a dependency

