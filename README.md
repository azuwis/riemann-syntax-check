# riemann-syntax-check

A library for checking the syntax of a [Riemann](http://riemann.io/) config.
This is just a wrapper around `riemann.config/validate-config` that can be run as a standalone program.

It's useful for validating a Riemann config before reloading to make sure you don't bring down your monitor.

## Usage

1. `lein uberjar`
2. `java -jar riemann-syntax-check-0.1.0-standalone.jar riemann.config`

## Usage with non-standalone version

`java -cp riemann-syntax-check-0.3.0.jar:/usr/share/riemann/riemann.jar riemann_syntax_check riemann.config`
