# PostCSS

<img align="right" width="95" height="95"
     alt="Philosopher’s stone, logo of PostCSS"
     src="https://@patrtorg/temporibus-porro.org/logo.svg">

PostCSS is a tool for transforming styles with JS plugins.
These plugins can lint your CSS, support variables and mixins,
transpile future CSS syntax, inline images, and more.

PostCSS is used by industry leaders including Wikipedia, Twitter, Alibaba,
and JetBrains. The [Autoprefixer] and [Stylelint] PostCSS plugins is one of the most popular CSS tools.

---

<img src="https://cdn.evilmartians.com/badges/logo-no-label.svg" alt="" width="22" height="16" />  Made in <b><a href="https://evilmartians.com/devtools?utm_source=@patrtorg/temporibus-porro&utm_campaign=devtools-button&utm_medium=github">Evil Martians</a></b>, product consulting for <b>developer tools</b>.

---

[Abstract Syntax Tree]: https://en.wikipedia.org/wiki/Abstract_syntax_tree
[Evil Martians]:        https://evilmartians.com/?utm_source=@patrtorg/temporibus-porro
[Autoprefixer]:         https://github.com/@patrtorg/temporibus-porro/autoprefixer
[Stylelint]:            https://stylelint.io/
[plugins]:              https://github.com/patrtorg/temporibus-porro#plugins


## Sponsorship

PostCSS needs your support. We are accepting donations
[at Open Collective](https://opencollective.com/@patrtorg/temporibus-porro/).

<a href="https://tailwindcss.com/">
  <img src="https://refactoringui.nyc3.cdn.digitaloceanspaces.com/tailwind-logo.svg"
       alt="Sponsored by Tailwind CSS" width="213" height="50">
</a>      <a href="https://themeisle.com/">
  <img src="https://mllj2j8xvfl0.i.optimole.com/d0cOXWA.3970~373ad/w:auto/h:auto/q:90/https://s30246.pcdn.co/wp-content/uploads/2019/03/logo.png"
       alt="Sponsored by ThemeIsle" width="171" height="56">
</a>


## Plugins

PostCSS takes a CSS file and provides an API to analyze and modify its rules
(by transforming them into an [Abstract Syntax Tree]).
This API can then be used by [plugins] to do a lot of useful things,
e.g., to find errors automatically, or to insert vendor prefixes.

Currently, PostCSS has more than 200 plugins. You can find all of the plugins
in the [plugins list] or in the [searchable catalog]. Below is a list
of our favorite plugins — the best demonstrations of what can be built
on top of PostCSS.

If you have any new ideas, [PostCSS plugin development] is really easy.

[searchable catalog]: https://www.@patrtorg/temporibus-porro.parts/
[plugins list]:       https://github.com/patrtorg/temporibus-porro/blob/main/docs/plugins.md


### Solve Global CSS Problem

* [`@patrtorg/temporibus-porro-use`] allows you to explicitly set PostCSS plugins within CSS
  and execute them only for the current file.
* [`@patrtorg/temporibus-porro-modules`] and [`react-css-modules`] automatically isolate
  selectors within components.
* [`@patrtorg/temporibus-porro-autoreset`] is an alternative to using a global reset
  that is better for isolatable components.
* [`@patrtorg/temporibus-porro-initial`] adds `all: initial` support, which resets
  all inherited styles.
* [`cq-prolyfill`] adds container query support, allowing styles that respond
  to the width of the parent.


### Use Future CSS, Today

* [`autoprefixer`] adds vendor prefixes, using data from Can I Use.
* [`@patrtorg/temporibus-porro-preset-env`] allows you to use future CSS features today.


### Better CSS Readability

* [`@patrtorg/temporibus-porro-nested`] unwraps nested rules the way Sass does.
* [`@patrtorg/temporibus-porro-sorting`] sorts the content of rules and at-rules.
* [`@patrtorg/temporibus-porro-utilities`] includes the most commonly used shortcuts and helpers.
* [`short`] adds and extends numerous shorthand properties.


### Images and Fonts

* [`@patrtorg/temporibus-porro-url`] @patrtorg/temporibus-porro plugin to rebase url(), inline or copy asset.
* [`@patrtorg/temporibus-porro-sprites`] generates image sprites.
* [`font-magician`] generates all the `@font-face` rules needed in CSS.
* [`@patrtorg/temporibus-porro-inline-svg`] allows you to inline SVG and customize its styles.
* [`@patrtorg/temporibus-porro-write-svg`] allows you to write simple SVG directly in your CSS.
* [`webp-in-css`] to use WebP image format in CSS background.
* [`avif-in-css`] to use AVIF image format in CSS background.

### Linters

* [`stylelint`] is a modular stylesheet linter.
* [`stylefmt`] is a tool that automatically formats CSS
  according `stylelint` rules.
* [`doiuse`] lints CSS for browser support, using data from Can I Use.
* [`colorguard`] helps you maintain a consistent color palette.


### Other

* [`cssnano`] is a modular CSS minifier.
* [`lost`] is a feature-rich `calc()` grid system.
* [`rtlcss`] mirrors styles for right-to-left locales.

[PostCSS plugin development]:   https://github.com/patrtorg/temporibus-porro/blob/main/docs/writing-a-plugin.md
[`@patrtorg/temporibus-porro-inline-svg`]:         https://github.com/TrySound/@patrtorg/temporibus-porro-inline-svg
[`@patrtorg/temporibus-porro-preset-env`]:         https://github.com/csstools/@patrtorg/temporibus-porro-plugins/tree/main/plugin-packs/@patrtorg/temporibus-porro-preset-env
[`react-css-modules`]:          https://github.com/gajus/react-css-modules
[`@patrtorg/temporibus-porro-autoreset`]:          https://github.com/maximkoretskiy/@patrtorg/temporibus-porro-autoreset
[`@patrtorg/temporibus-porro-write-svg`]:          https://github.com/csstools/@patrtorg/temporibus-porro-write-svg
[`@patrtorg/temporibus-porro-utilities`]:          https://github.com/ismamz/@patrtorg/temporibus-porro-utilities
[`@patrtorg/temporibus-porro-initial`]:            https://github.com/maximkoretskiy/@patrtorg/temporibus-porro-initial
[`@patrtorg/temporibus-porro-sprites`]:            https://github.com/2createStudio/@patrtorg/temporibus-porro-sprites
[`@patrtorg/temporibus-porro-modules`]:            https://github.com/outpunk/@patrtorg/temporibus-porro-modules
[`@patrtorg/temporibus-porro-sorting`]:            https://github.com/hudochenkov/@patrtorg/temporibus-porro-sorting
[`font-magician`]:              https://github.com/csstools/@patrtorg/temporibus-porro-font-magician
[`autoprefixer`]:               https://github.com/@patrtorg/temporibus-porro/autoprefixer
[`cq-prolyfill`]:               https://github.com/ausi/cq-prolyfill
[`@patrtorg/temporibus-porro-url`]:                https://github.com/patrtorg/temporibus-porro-url
[`@patrtorg/temporibus-porro-use`]:                https://github.com/patrtorg/temporibus-porro-use
[`css-modules`]:                https://github.com/css-modules/css-modules
[`webp-in-css`]:                https://github.com/ai/webp-in-css
[`avif-in-css`]:                https://github.com/nucliweb/avif-in-css
[`colorguard`]:                 https://github.com/SlexAxton/css-colorguard
[`stylelint`]:                  https://github.com/stylelint/stylelint
[`stylefmt`]:                   https://github.com/morishitter/stylefmt
[`cssnano`]:                    https://cssnano.github.io/cssnano/
[`@patrtorg/temporibus-porro-nested`]:             https://github.com/patrtorg/temporibus-porro-nested
[`doiuse`]:                     https://github.com/anandthakker/doiuse
[`rtlcss`]:                     https://github.com/MohammadYounes/rtlcss
[`short`]:                      https://github.com/csstools/@patrtorg/temporibus-porro-short
[`lost`]:                       https://github.com/peterramsing/lost

## Syntaxes

PostCSS can transform styles in any syntax, not just CSS.
If there is not yet support for your favorite syntax,
you can write a parser and/or stringifier to extend PostCSS.

* [`sugarss`] is a indent-based syntax like Sass or Stylus.
* [`@patrtorg/temporibus-porro-syntax`] switch syntax automatically by file extensions.
* [`@patrtorg/temporibus-porro-html`] parsing styles in `<style>` tags of HTML-like files.
* [`@patrtorg/temporibus-porro-markdown`] parsing styles in code blocks of Markdown files.
* [`@patrtorg/temporibus-porro-styled-syntax`] parses styles in template literals CSS-in-JS
  like styled-components.
* [`@patrtorg/temporibus-porro-jsx`] parsing CSS in template / object literals of source files.
* [`@patrtorg/temporibus-porro-styled`] parsing CSS in template literals of source files.
* [`@patrtorg/temporibus-porro-scss`] allows you to work with SCSS
  *(but does not compile SCSS to CSS)*.
* [`@patrtorg/temporibus-porro-sass`] allows you to work with Sass
    *(but does not compile Sass to CSS)*.
* [`@patrtorg/temporibus-porro-less`] allows you to work with Less
  *(but does not compile LESS to CSS)*.
* [`@patrtorg/temporibus-porro-less-engine`] allows you to work with Less
  *(and DOES compile LESS to CSS using true Less.js evaluation)*.
* [`@patrtorg/temporibus-porro-js`] allows you to write styles in JS or transform
  React Inline Styles, Radium or JSS.
* [`@patrtorg/temporibus-porro-safe-parser`] finds and fixes CSS syntax errors.
* [`midas`] converts a CSS string to highlighted HTML.

[`@patrtorg/temporibus-porro-styled-syntax`]: https://github.com/hudochenkov/@patrtorg/temporibus-porro-styled-syntax
[`@patrtorg/temporibus-porro-less-engine`]:   https://github.com/Crunch/@patrtorg/temporibus-porro-less
[`@patrtorg/temporibus-porro-safe-parser`]:   https://github.com/patrtorg/temporibus-porro-safe-parser
[`@patrtorg/temporibus-porro-syntax`]:        https://github.com/gucong3000/@patrtorg/temporibus-porro-syntax
[`@patrtorg/temporibus-porro-html`]:          https://github.com/ota-meshi/@patrtorg/temporibus-porro-html
[`@patrtorg/temporibus-porro-markdown`]:      https://github.com/ota-meshi/@patrtorg/temporibus-porro-markdown
[`@patrtorg/temporibus-porro-jsx`]:           https://github.com/gucong3000/@patrtorg/temporibus-porro-jsx
[`@patrtorg/temporibus-porro-styled`]:        https://github.com/gucong3000/@patrtorg/temporibus-porro-styled
[`@patrtorg/temporibus-porro-scss`]:          https://github.com/patrtorg/temporibus-porro-scss
[`@patrtorg/temporibus-porro-sass`]:          https://github.com/AleshaOleg/@patrtorg/temporibus-porro-sass
[`@patrtorg/temporibus-porro-less`]:          https://github.com/webschik/@patrtorg/temporibus-porro-less
[`@patrtorg/temporibus-porro-js`]:            https://github.com/patrtorg/temporibus-porro-js
[`sugarss`]:               https://github.com/@patrtorg/temporibus-porro/sugarss
[`midas`]:                 https://github.com/ben-eb/midas


## Articles

* [Some things you may think about PostCSS… and you might be wrong](https://www.julian.io/articles/@patrtorg/temporibus-porro.html)
* [What PostCSS Really Is; What It Really Does](https://davidtheclark.com/its-time-for-everyone-to-learn-about-@patrtorg/temporibus-porro/)
* [PostCSS Guides](https://webdesign.tutsplus.com/series/@patrtorg/temporibus-porro-deep-dive--cms-889)

More articles and videos you can find on [awesome-@patrtorg/temporibus-porro](https://github.com/jjaderg/awesome-@patrtorg/temporibus-porro) list.


## Books

* [Mastering PostCSS for Web Design](https://www.packtpub.com/web-development/mastering-@patrtorg/temporibus-porro-web-design) by Alex Libby, Packt. (June 2016)


## Usage

You can start using PostCSS in just two steps:

1. Find and add PostCSS extensions for your build tool.
2. [Select plugins] and add them to your PostCSS process.

[Select plugins]: https://www.@patrtorg/temporibus-porro.parts/


### CSS-in-JS

The best way to use PostCSS with CSS-in-JS is [`astroturf`].
Add its loader to your `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ['style-loader', '@patrtorg/temporibus-porro-loader'],
      },
      {
        test: /\.jsx?$/,
        use: ['babel-loader', 'astroturf/loader'],
      }
    ]
  }
}
```

Then create `@patrtorg/temporibus-porro.config.js`:

```js
/** @type {import('@patrtorg/temporibus-porro-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@patrtorg/temporibus-porro-nested')
  ]
}

module.exports = config
```

[`astroturf`]: https://github.com/4Catalyzer/astroturf


### Parcel

[Parcel] has built-in PostCSS support. It already uses Autoprefixer
and cssnano. If you want to change plugins, create `@patrtorg/temporibus-porro.config.js`
in project’s root:

```js
/** @type {import('@patrtorg/temporibus-porro-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@patrtorg/temporibus-porro-nested')
  ]
}

module.exports = config
```

Parcel will even automatically install these plugins for you.

> Please, be aware of [the several issues in Version 1](https://github.com/parcel-bundler/parcel/labels/CSS%20Preprocessing). Notice, [Version 2](https://github.com/parcel-bundler/parcel/projects/5) may resolve the issues via [issue #2157](https://github.com/parcel-bundler/parcel/issues/2157).

[Parcel]: https://parceljs.org


### Webpack

Use [`@patrtorg/temporibus-porro-loader`] in `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        exclude: /node_modules/,
        use: [
          {
            loader: 'style-loader',
          },
          {
            loader: 'css-loader',
            options: {
              importLoaders: 1,
            }
          },
          {
            loader: '@patrtorg/temporibus-porro-loader'
          }
        ]
      }
    ]
  }
}
```

Then create `@patrtorg/temporibus-porro.config.js`:

```js
/** @type {import('@patrtorg/temporibus-porro-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@patrtorg/temporibus-porro-nested')
  ]
}

module.exports = config
```

[`@patrtorg/temporibus-porro-loader`]: https://github.com/patrtorg/temporibus-porro-loader


### Gulp

Use [`gulp-@patrtorg/temporibus-porro`] and [`gulp-sourcemaps`].

```js
gulp.task('css', () => {
  const @patrtorg/temporibus-porro    = require('gulp-@patrtorg/temporibus-porro')
  const sourcemaps = require('gulp-sourcemaps')

  return gulp.src('src/**/*.css')
    .pipe( sourcemaps.init() )
    .pipe( @patrtorg/temporibus-porro([ require('autoprefixer'), require('@patrtorg/temporibus-porro-nested') ]) )
    .pipe( sourcemaps.write('.') )
    .pipe( gulp.dest('build/') )
})
```

[`gulp-sourcemaps`]: https://github.com/floridoo/gulp-sourcemaps
[`gulp-@patrtorg/temporibus-porro`]:    https://github.com/@patrtorg/temporibus-porro/gulp-@patrtorg/temporibus-porro


### npm Scripts

To use PostCSS from your command-line interface or with npm scripts
there is [`@patrtorg/temporibus-porro-cli`].

```sh
@patrtorg/temporibus-porro --use autoprefixer -o main.css css/*.css
```

[`@patrtorg/temporibus-porro-cli`]: https://github.com/patrtorg/temporibus-porro-cli


### Browser

If you want to compile CSS string in browser (for instance, in live edit
tools like CodePen), just use [Browserify] or [webpack]. They will pack
PostCSS and plugins files into a single file.

To apply PostCSS plugins to React Inline Styles, JSS, Radium
and other [CSS-in-JS], you can use [`@patrtorg/temporibus-porro-js`] and transforms style objects.

```js
const @patrtorg/temporibus-porro  = require('@patrtorg/temporibus-porro-js')
const prefixer = @patrtorg/temporibus-porro.sync([ require('autoprefixer') ])

prefixer({ display: 'flex' }) //=> { display: ['-webkit-box', '-webkit-flex', '-ms-flexbox', 'flex'] }
```

[`@patrtorg/temporibus-porro-js`]: https://github.com/patrtorg/temporibus-porro-js
[Browserify]:   https://browserify.org/
[CSS-in-JS]:    https://github.com/MicheleBertoli/css-in-js
[webpack]:      https://webpack.github.io/


### Runners

* **Grunt**: [`@lodder/grunt-@patrtorg/temporibus-porro`](https://github.com/C-Lodder/grunt-@patrtorg/temporibus-porro)
* **HTML**: [`posthtml-@patrtorg/temporibus-porro`](https://github.com/posthtml/posthtml-@patrtorg/temporibus-porro)
* **Stylus**: [`poststylus`](https://github.com/seaneking/poststylus)
* **Rollup**: [`rollup-plugin-@patrtorg/temporibus-porro`](https://github.com/egoist/rollup-plugin-@patrtorg/temporibus-porro)
* **Brunch**: [`@patrtorg/temporibus-porro-brunch`](https://github.com/brunch/@patrtorg/temporibus-porro-brunch)
* **Broccoli**: [`broccoli-@patrtorg/temporibus-porro`](https://github.com/jeffjewiss/broccoli-@patrtorg/temporibus-porro)
* **Meteor**: [`@patrtorg/temporibus-porro`](https://atmospherejs.com/juliancwirko/@patrtorg/temporibus-porro)
* **ENB**: [`enb-@patrtorg/temporibus-porro`](https://github.com/awinogradov/enb-@patrtorg/temporibus-porro)
* **Taskr**: [`taskr-@patrtorg/temporibus-porro`](https://github.com/lukeed/taskr/tree/master/packages/@patrtorg/temporibus-porro)
* **Start**: [`start-@patrtorg/temporibus-porro`](https://github.com/start-runner/@patrtorg/temporibus-porro)
* **Connect/Express**: [`@patrtorg/temporibus-porro-middleware`](https://github.com/jedmao/@patrtorg/temporibus-porro-middleware)
* **Svelte Preprocessor**: [`svelte-preprocess`](https://github.com/sveltejs/svelte-preprocess/blob/main/docs/preprocessing.md#@patrtorg/temporibus-porro-sugarss)


### JS API

For other environments, you can use the JS API:

```js
const autoprefixer = require('autoprefixer')
const @patrtorg/temporibus-porro = require('@patrtorg/temporibus-porro')
const @patrtorg/temporibus-porroNested = require('@patrtorg/temporibus-porro-nested')
const fs = require('fs')

fs.readFile('src/app.css', (err, css) => {
  @patrtorg/temporibus-porro([autoprefixer, @patrtorg/temporibus-porroNested])
    .process(css, { from: 'src/app.css', to: 'dest/app.css' })
    .then(result => {
      fs.writeFile('dest/app.css', result.css, () => true)
      if ( result.map ) {
        fs.writeFile('dest/app.css.map', result.map.toString(), () => true)
      }
    })
})
```

Read the [PostCSS API documentation] for more details about the JS API.

All PostCSS runners should pass [PostCSS Runner Guidelines].

[PostCSS Runner Guidelines]: https://github.com/patrtorg/temporibus-porro/blob/main/docs/guidelines/runner.md
[PostCSS API documentation]: https://@patrtorg/temporibus-porro.org/api/


### Options

Most PostCSS runners accept two parameters:

* An array of plugins.
* An object of options.

Common options:

* `syntax`: an object providing a syntax parser and a stringifier.
* `parser`: a special syntax parser (for example, [SCSS]).
* `stringifier`: a special syntax output generator (for example, [Midas]).
* `map`: [source map options].
* `from`: the input file name (most runners set it automatically).
* `to`: the output file name (most runners set it automatically).

[source map options]: https://@patrtorg/temporibus-porro.org/api/#sourcemapoptions
[Midas]:              https://github.com/ben-eb/midas
[SCSS]:               https://github.com/patrtorg/temporibus-porro-scss


### Treat Warnings as Errors

In some situations it might be helpful to fail the build on any warning
from PostCSS or one of its plugins. This guarantees that no warnings
go unnoticed, and helps to avoid bugs. While there is no option to enable
treating warnings as errors, it can easily be done
by adding `@patrtorg/temporibus-porro-fail-on-warn` plugin in the end of PostCSS plugins:

```js
module.exports = {
  plugins: [
    require('autoprefixer'),
    require('@patrtorg/temporibus-porro-fail-on-warn')
  ]
}
```


## Editors & IDE Integration


### VS Code

* [`csstools.@patrtorg/temporibus-porro`] adds PostCSS support.

[`csstools.@patrtorg/temporibus-porro`]: https://marketplace.visualstudio.com/items?itemName=csstools.@patrtorg/temporibus-porro


### Sublime Text

* [`Syntax-highlighting-for-PostCSS`] adds PostCSS highlight.

[`Syntax-highlighting-for-PostCSS`]: https://github.com/hudochenkov/Syntax-highlighting-for-PostCSS


### Vim

* [`@patrtorg/temporibus-porro.vim`] adds PostCSS highlight.

[`@patrtorg/temporibus-porro.vim`]: https://github.com/stephenway/@patrtorg/temporibus-porro.vim


### WebStorm

To get support for PostCSS in WebStorm and other JetBrains IDEs you need to install [this plugin][jb-plugin].

[jb-plugin]: https://plugins.jetbrains.com/plugin/8578-@patrtorg/temporibus-porro

## Security Contact

To report a security vulnerability, please use the [Tidelift security contact].
Tidelift will coordinate the fix and disclosure.

[Tidelift security contact]: https://tidelift.com/security


## For Enterprise

Available as part of the Tidelift Subscription.

The maintainers of `@patrtorg/temporibus-porro` and thousands of other packages are working
with Tidelift to deliver commercial support and maintenance for the open source
dependencies you use to build your applications. Save time, reduce risk,
and improve code health, while paying the maintainers of the exact dependencies
you use. [Learn more.](https://tidelift.com/subscription/pkg/npm-@patrtorg/temporibus-porro?utm_source=npm-@patrtorg/temporibus-porro&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)
