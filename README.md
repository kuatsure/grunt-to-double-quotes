# grunt-to-double-quotes

[![Build Status](https://travis-ci.org/kuatsure/grunt-to-double-quotes.png?branch=master)](https://travis-ci.org/kuatsure/grunt-to-double-quotes) [![Dependency Status](https://david-dm.org/kuatsure/grunt-to-double-quotes.png?theme=shields.io)](https://david-dm.org/kuatsure/grunt-to-double-quotes) [![Built with Grunt](https://cdn.gruntjs.com/builtwith.png)](http://gruntjs.com/)

> Replaces single ( escaped or otherwise ) quotes with double quotes.

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-to-double-quotes --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-to-double-quotes');
```

## The "to_double_quotes" task

### Overview
In your project's Gruntfile, add a section named `to_double_quotes` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  to_double_quotes: {
    your_target: {
      // Target-specific file lists go here.
    },
  },
})
```

### Options

None.

### Usage Examples

#### Default Options

Removes single quotes from files while concatting.

```js
grunt.initConfig({
  to_double_quotes: {
    files: {
      'dest/default_options': ['src/testing', 'src/123'],
    },
  },
})
```

Results: `'Hi there!'` -> `"Hi there!"`

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## License
Copyright (c) 2014 Jarrett Drouillard. Licensed under the MIT license.
