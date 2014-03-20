# Foundation libsass template

This is a template to start your own project using:

  * [Gulp](http://gulpjs.com)
  * [Foundation](http://foundation.zurb.com) + libsass
  * [Autoprefixer]()
  * [CSSO](http://bem.info/tools/optimizers/csso/) and [UglifyJS2](http://lisperator.net/uglifyjs/)
  * [JSHint](http://www.jshint.com/)
  * [BrowserSync](http://browsersync.io/)

## Requirements

You'll need to have the following items installed before continuing.

  * [Node.js](http://nodejs.org): Use the installer provided on the NodeJS website.
  * [Gulp](http://gulpjs.com): Run `[sudo] npm install -g gulp`
  * [Bower](http://bower.io): Run `[sudo] npm install -g bower`

## Quickstart

```bash
git clone https://github.com/covertg/libsass-template.git
npm install
bower install
```

While you're working on your project, run:

```bash
gulp
```

And you're set! Gulp will run, watch your changes, and serve your files on localhost. Check the console output for more info.

## Directory Structure

  * `src/`: All application sources go here
  * `build/`: All built files go here
  * `bower_components/foundation/scss/foundation/_settings.scss`: Foundation configuration settings go in here
  * `Gulpfile.js`: Check this out for a sense of what's going on

## Other Notes

  * Replace the ">=" operators with "^" in package.json in the case of future API updates or other package breakages.
  * To build once for production, run: `gulp build --type dist` and gulp will rebuild and optimize/minify your files.
  * Currently, we are using a PR repo for autoprefixer because it's up-to-date.
  * NPM may seem to hang when installing ws (dependency of BrowserSync). Just give it some time.