# Express App using Electrolyte

This example illustrates how to use [Electrolyte](https://github.com/jaredhanson/electrolyte)
when building a web application with [Express](http://expressjs.com/).

Electrolyte uses dependency injection to automatically initialize the database
connection, logging facility, and other components needed by route handlers.
This eliminates boilerplate plumbing, and results in very modular route
handlers.

When writing unit tests, any component required by a route handler can easily be
mocked, allowing for maximum code coverage, including easy simulation of errors
and error handling.

#### Install & Run

    $ npm install
    $ npm start

#### Directory Structure

- [app/index.js](app/index.js)  creates an Express application
- [app/routes.js](app/routes.js)  routes drawn by application
- [app/handers/](app/handlers/)  handlers for HTTP requests
- [app/components/](app/components/)  components needed by application
- [etc/init/](etc/init/)   application initializers
