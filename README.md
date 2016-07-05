[![Build Status](https://travis-ci.org/mrstebo/node-env-config-loader.svg?branch=master)](https://travis-ci.org/mrstebo/node-env-config-loader)

# node-env-config-loader
Library for loading configuration files that you can inject environment variables in to.

This library will replace `#{MY_ENVIRONMENT_VARIABLE}` with your environment variable of the same name.

## How do I use this?

### The `load` function

All you need to do is send a file path to the `load` function and it will handle everything for you.

_JSON and YAML files are the only file types currently supported_

```js
var configLoader = require('node-env-config-loader');
var config = configLoader.load('./config.yml');
```
