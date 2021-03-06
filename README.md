# cljs-lein-npm-figw-ex

Built on example from:
https://github.com/kissaten/cljs-lein-npm-example
Attempting to modify for basic example with re-frame instead of reagent.

The readme for that file is provided below:

Note, another version of this which seems to have been updated less recently than the above model is:
https://github.com/njordhov/cljsnode

# cljs lein-npm example

Clojurescript based reference SPA on Heroku using node express, bootstrap,
reactjs/reagent and Kioo templates, demonstrating "isomorphic" clojurescript
shared between frontend and backend and Figwheel hotloading code changes
to both.

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

Fork on github as a starting point for your own projects.
A goal is to turn this into a Leiningen template.

## Run Locally

To start a server on your own computer:

    lein do clean, deps, compile
    lein run

Point your browser to the displayed local port.
Click on the displayed text to refresh.

## Deploy to Heroku

To start a server on Heroku:

    heroku create <new app name>
    git push heroku main
    heroku open

This will open the site in your browser.

## Development Workflow

Start figwheel for interactive development with
automatic builds and code loading:

    lein figwheel app server

Wait until Figwheel is ready to connect, then
start a server in another terminal:

    lein run

Open the displayed URL in a browser.
Figwheel will push code changes to the app and server.

## License

Copyright © 2015 Terje Norderhaug

Based on an app concept by Marian Schubert.

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.

# Update (21/02/22)

## 1

To get to run locally, needed to add a dependency to the project file as per:
https://stackoverflow.com/questions/56779380/clojure-lein-figwheel-and-classnotfoundexception-javax-xml-bind-datatypeconver
