# assemble-middleware-navigation [![NPM version](https://badge.fury.io/js/assemble-middleware-navigation.png)](http://badge.fury.io/js/assemble-middleware-navigation)

> Assemble navigation middleware. Automatically generate Bootstrap-style, multi-level side nav. See the sidenav on assemble.io for a demonstration.

**Upgrade notice!**: as of v0.1.0, _this middlweare requires Assemble v0.5.0._

_Get the [Assemble generator](https://github.com/assemble/generator-assemble) for Yeoman to kickstart new Assemble projects using this middleware._

**Here's a preview**

![image](https://f.cloud.github.com/assets/383994/2523672/94f62414-b4d4-11e3-98c6-fc3c07bef4b4.png)

***

## Quickstart
Install with [npm](npmjs.org):

```bash
npm i assemble-middleware-navigation --save-dev
```


## Usage
Register the middleware with Assemble:

```js
options: {
  middleware: ['assemble-middleware-navigation', 'foo/*.js']
}
```

Visit the [middleware docs](http://assemble.io/plugins/) for more info or for help getting started.

Add this markup where you want the navigation:

```html
<div id="navigation">
  <!-- navigation -->
</div>
```

The plugin uses page headings to construct the nav items, results in something like:

```html
<div id="navigation">
  <!-- navigation -->
  <ul class="nav sidenav">
    <li><a href="#collections">Collections</a>
      <ul class="nav">
        <li> <a href="#collections-after">{{after}}</a> </li>
        <li> <a href="#collections-any">{{any}}</a> </li>
        <li> <a href="#collections-before">{{before}}</a> </li>
      </ul>
    </li>
  </ul>
</div>
```

***

## Other Assemble middleware
Here are some related projects you might be interested in from the [Assemble](http://assemble.io) core team.

+ [assemble-middleware-anchors](https://api.github.com/repos/assemble/assemble-middleware-anchors): Assemble middleware for creating anchor tags from generated html. 
+ [assemble-middleware-contextual](https://api.github.com/repos/assemble/assemble-middleware-contextual): Assemble middleware for generating a JSON file containing the context of each page. Basic middleware to help see what's happening in the build. 
+ [assemble-middleware-decompress](https://api.github.com/repos/assemble/assemble-middleware-decompress): Assemble plugin for extracting zip, tar and tar.gz archives.  
+ [assemble-middleware-download](https://api.github.com/repos/assemble/assemble-middleware-download): Assemble middleware for downloading files from GitHub. 
+ [assemble-middleware-lunr](https://api.github.com/repos/assemble/assemble-middleware-lunr): Assemble middleware for creating a search engine within your static site using lunr.js. 
+ [assemble-middleware-permalinks](https://api.github.com/repos/assemble/assemble-middleware-permalinks): Permalinks middleware for Assemble, the static site generator for Grunt.js and Yeoman. This plugin enables powerful and configurable URI replacement patterns, presets, uses Moment.js for parsing dates, and much more. 
+ [assemble-middleware-toc](https://api.github.com/repos/assemble/assemble-middleware-toc): Assemble middleware for creating a table of contents in the generated HTML, using Cheerio.js 
+ [assemble-middleware-wordcount](https://api.github.com/repos/assemble/assemble-middleware-wordcount): Assemble middleware for displaying a word-count, and estimated reading time on blog posts or pages.  

Visit [assemble.io/assemble-middleware](http:/assemble.io/assemble-middleware/) for more information about [Assemble](http:/assemble.io/) middleware.


## Contributing
Find a bug? Have a feature request? Please [create an Issue](https://github.com/assemble/assemble-middleware-navigation/issues).

In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality,
and run `docs` in the command line to build the docs with [Verb](https://github.com/assemble/verb).

Pull requests are also encouraged, and if you find this project useful please consider "starring" it to show your support! Thanks!

## Authors

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on May 03, 2014._
