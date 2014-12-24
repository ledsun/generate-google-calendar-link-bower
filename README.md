# generate-google-calendar-link-bower

A bower package of [generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link).

[generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link)のbowerパッケージです。

[![Build Status](https://travis-ci.org/ledsun/generate-google-calendar-link.svg)](https://travis-ci.org/ledsun/generate-google-calendar-link-bower)

[![Sauce Test Status](https://saucelabs.com/browser-matrix/generate-google-calendar-link.svg)](https://saucelabs.com/u/generate-google-calendar-link-bower)

## Setup

```
bower install generate-google-calendar-link
```

htmlにscriptタグを埋め込みます。
```html
<link rel="stylesheet" href="bower_components/generate-google-calendar-link/index.css">
<div id="result"></div>
<script src="bower_components/generate-google-calendar-link/index.js"></script>
<script>
var a = generateLink({
    start: new Date(2014, 10, 15, 10),
    end: new Date(2014, 10, 15, 18),
    title: 'New event',
    location: 'Some where',
    details: 'http://event.description.example.com/11234'
})

document.getElementById('result').appendChild(a)
</script>
```

## Contributing

contributeするには

1. Fork it.
1. Create a branch (git checkout -b my_function)
1. Commit your changes (git commit -am "Added My Function")
1. Push to the branch (git push origin my_function)
1. Open a Pull Request
1. Enjoy a refreshing coffe and wait

### Build

```
npm install
npm run build
```

The main function in `src/generate-google-calendar-link.js`.

主な関数は`src/generate-google-calendar-link.js`に入っています。

`src/generate-google-calendar-link.js` is converted by [browserify](http://browserify.org/).

`src/generate-google-calendar-link.js`を[browserify](http://browserify.org/)使って変換します。

### Testing
#### browser

Open `example.html` to check `index.js` is loadable by a browser.

ブラウザで読み込めるか確認するには、`example.html`を開きます。

```
open example.js
```


[zuul](https://github.com/defunctzombie/zuul) is used to check `index.js` works in corss borwsers.

クロスブラウザで動作するか確認するには、[zuul](https://github.com/defunctzombie/zuul)を使います。

```
npm run browser
```

### Deploy

Update `package.json`.

`package.json`を更新します。

```
npm install
npm run build
npm test
npm publish
```
