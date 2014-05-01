# assemble-contrib-navigation [![NPM version](https://badge.fury.io/js/assemble-contrib-navigation.png)](http://badge.fury.io/js/assemble-contrib-navigation)

> Assemble plugin to automatically generate Bootstrap-style, multi-level side navigation. See the sidenav on assemble.io for a demonstration.

**Heads up!** v0.1.0 and greater requires Assemble v0.5.0!

_Get the [Assemble generator](https://github.com/assemble/generator-assemble) for Yeoman to kickstart new Assemble projects using this plugin._

**Here's a preview**

![image](https://f.cloud.github.com/assets/383994/2523672/94f62414-b4d4-11e3-98c6-fc3c07bef4b4.png)

***

## Quickstart
Install with [npm](npmjs.org):

```bash
npm i assemble-contrib-navigation --save-dev
```


## Usage
Register the plugin with Assemble:

```js
options: {
  plugins: ['assemble-contrib-navigation', 'foo/*.js']
}
```

Visit the [plugins docs](http://assemble.io/plugins/) for more info or for help getting started.

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

## Assemble plugins
Here are some related projects you might be interested in from the [Assemble](http://assemble.io) core team.

+ [assemble-plugin-drafts](https://api.github.com/repos/assemble/assemble-plugin-drafts): Assemble plugin (v0.5.0) for preventing drafts from being rendered. 
+ [assemble-plugin-pagination](https://api.github.com/repos/assemble/assemble-plugin-pagination): WIP this plugin isn't ready for use! 
+ [assemble-plugin-rss](https://api.github.com/repos/assemble/assemble-plugin-rss): NOT Published yet! This plugin isn't ready for prime time! Plugin for creating RSS feeds with Assemble, the static site generator for Node.js, Grunt.js and Yeoman.  
+ [generator-plugin](https://api.github.com/repos/assemble/generator-plugin): Yeoman generator for Assemble plugins.  
+ [grunt-init-assemble-plugin](https://api.github.com/repos/assemble/grunt-init-assemble-plugin): Generate a plugin for Assemble. 
+ [plugins](https://api.github.com/repos/assemble/plugins): Collection of contrib plugins maintained by the Assemble core team. 
+ [assemble-contrib-lunr](https://api.github.com/repos/assemble/assemble-contrib-lunr): Assemble plugin for creating a search engine within your static site using lunr.js. 
+ [assemble-contrib-lunr-examples](https://api.github.com/repos/assemble/assemble-contrib-lunr-examples): Usages examples for assemble-contrib-lunr, a search plugin for Assemble. 
+ [assemble-contrib-markdown](https://api.github.com/repos/assemble/assemble-contrib-markdown): HEADS UP! This isn't ready for prime time! Convert markdown files to HTML using marked.js. This plugin is an alternative to Assemble's markdown Handlebars helpers. Both are useful in different scenarios. 
+ [assemble-contrib-navigation](https://api.github.com/repos/assemble/assemble-contrib-navigation): Assemble plugin for automatically generating Bootstrap-style side navigation.  
+ [assemble-contrib-permalinks](https://api.github.com/repos/assemble/assemble-contrib-permalinks): Permalinks plugin for Assemble, the static site generator for Grunt.js and Yeoman. This plugin enables powerful and configurable URI replacement patterns, presets, uses Moment.js for parsing dates, and much more. 
+ [assemble-contrib-sitemap](https://api.github.com/repos/assemble/assemble-contrib-sitemap): Sitemap generator plugin for Assemble 
+ [assemble-contrib-toc](https://api.github.com/repos/assemble/assemble-contrib-toc): Create a table of contents in the generated HTML, using Cheerio.js 
+ [assemble-contrib-toc-example](https://api.github.com/repos/assemble/assemble-contrib-toc-example): Example for generating a Table of Contents using Assemble. 
+ [assemble-contrib-wordcount](https://api.github.com/repos/assemble/assemble-contrib-wordcount): Assemble plugin for displaying a word-count on blog posts or pages. 

Visit [assemble.io/plugins](http:/assemble.io/plugins/) for more information about [Assemble](http:/assemble.io/) plugins.


## Contributing
Find a bug? Have a feature request? Please [create an Issue](https://github.com/assemble/assemble-contrib-navigation/issues).

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

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on May 01, 2014._
