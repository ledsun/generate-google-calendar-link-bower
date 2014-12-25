# generate-google-calendar-link-bower

A bower package of [generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link).

[generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link)のbowerパッケージです。

## Desciption

[Browserify](http://browserify.org/) [generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link) to publish a bower package,
because [hyperscript](https://github.com/dominictarr/hyperscript) is not export a glabal object that is dependant libraries of [generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link).

[generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link)が依存している[hyperscript](https://github.com/dominictarr/hyperscript)はglobalオブジェクトを公開しません。 [generate-google-calendar-link](https://github.com/ledsun/generate-google-calendar-link)を[browserify](http://browserify.org/)で変換してbower packageとして公開します。


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

### Deploy

#### publish
Update verion in `bower.json`.

`bower.json`内のversionを更新します。

```
git add bower.json
git commit -m 'Release vX.X.X'
git tag 'vX.X.X'
git push origin master
git push origin 'vX.X.X'
```

#### confirm

```
cd test
bower cache clean
bower i generate-google-calendar-link
open confirm.html
```

Dose show a icon to add calendar?
