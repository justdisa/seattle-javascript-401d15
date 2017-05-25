![cf](http://i.imgur.com/7v5ASc8.png) 01: Node Ecosystem
=====================================

## Kickoff
* Intros
  * What do you want to do when you're done with 401?
* Canvas/Slack/Surveys/etc...
  * Calendar
  * YouTube link
  * General overview
* Pre-work: Great job!!
* Recap Career Development in 401
* Weekly pattern for 401JS - Mon-Thurs Code, Fri Career Dev
* Github - Course & Labs Repos
* TA / Instructor Support Workflow - Do your research...
* Lightning Talks & 1:1s
* Questions?

## Resources
* Read [modular patterns]
* Read [basic testing with mocha & chai]

## What is NodeJS?
  * **Overview**
    * open source JS framework
    * built for creating dynamic web applications
    * built on Chrome’s JS runtime, V8
    * V8 compiles JS to native machine code
    * code ran in the browser gets compiled in V8
    * written in C++ and JS
    * built for asynchronous I/O operations (using libuv)
    * utilizes an event driven, non-blocking architecture
    * lightweight and efficient
    * contains a rich ecosystem of available packages (NPM)

  * **NodeJS REPL**
    * Read, Evaluate, Print, Loop
    * great for testing simple javascript operations
    * global object in NodeJS: `global`

  * **Basics of Working in NodeJS**
    * `'use strict'` at the top of every file
    * **demo:**  simple file creation and execution

## Modular Patterns in NodeJS
  * **What is `require`?**
    * `require` is the function used to import modules in NodeJS
    * CommonJS defines a module format specification for creating modules in JS
    * AMD (Asynchronous Module Definition) loads modules and dependencies asynchronously

  * **Introduction to the `module.exports` Pattern**
    * `module.exports` vs `module.exports = exports = {}`
      * `module.exports` for exporting a single function
      * `module.exports = exports = {}` for exporting multiple methods
    * relative and absolute file paths
      * relative: relative to where you currently are in the file system
      * absolute: full file path
    * **demo:** hello world demo, modularized
    * **demo:** hello world demo, modularized, and with multiple methods

## Intro to Testing
  * **What is TDD?**
    * Test Driven Development
    * tests drive the development process
    * red, green, refactor

  * **What is BDD?**
    * Behavior Driven Development
    * behavior and specification that drives the development process
    * the lines are often unclear as to the differences between TDD/BDD - we adapt to both

  * **Working with MochaJS**
    * what is MochaJS?
      * feature rich JS test framework
      * gives us access to use `describe` and `it` blocks
    * globally install MochaJS: `npm install -g mocha`
    * what are assertions?
      * expressions that encapsulate logic and are evaluated in a targeted test
    * difference between unit, e2e, and integration testing
      * e2e: tests if the flow of an application, from start to finish, works as expected
      * unit: smallest testable parts of an application are tested
        * often testing features of other features
      * integration: phase of testing where individual modules are combined and tested as a group
      * **demo:** basic module testing
      * running mocha with a `/test` directory
      * using the `-w` watch flag

<!--links -->
[modular patterns]: https://docs.nodejitsu.com/articles/getting-started/what-is-require
[basic testing with mocha & chai]: http://code.tutsplus.com/tutorials/testing-in-nodejs--net-35018
