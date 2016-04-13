## [Autopolyfiller](https://github.com/azproduction/autopolyfiller) loader for [webpack](https://webpack.github.io/)


Heavily based on [deepsweet/autopolyfiller-loader](https://github.com/deepsweet/autopolyfiller-loader), but updated to work with newer versions of webpack.

> This is like [Autoprefixer](https://github.com/ai/autoprefixer), but for JavaScript polyfills. It scans your code and applies only required polyfills.

### Install

```sh
$ npm i -S autopolyfiller-webpack
```

### Usage

```js
module: {
    postLoaders: [ {
        test: /\.js$/,
        exclude: /\/(node_modules|bower_components)\//,
        loader: 'autopolyfiller-webpack',
        query: { browsers: [ 'last 2 versions', 'ie >= 9' ] }
    } ]
}
```

[Documentation: Using loaders](https://webpack.github.io/docs/using-loaders.html).

### License
[WTFPL](http://www.wtfpl.net/wp-content/uploads/2012/12/wtfpl-strip.jpg)
